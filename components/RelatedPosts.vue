<template>
	<section v-if="relatedPosts.length > 0">
		<h3>Related Posts</h3>
		<ul class="related">
			<li v-for="(post, i) of relatedPosts" :key="i" class="py-2 text-xs">
				<NuxtLink :title="post.title" :to="`/blog/${post.slug}/`">{{
					post.title
				}}</NuxtLink>
			</li>
		</ul>
	</section>
</template>
<script>
export default {
	props: {
		tags: {
			type: Array,
			required: true,
		},
		slug: {
			type: String,
			required: true,
		},
	},

	async fetch() {
		try {
			this.relatedPosts = await this.$content(`blog`, { deep: true })
				.only(['title', 'slug'])
				.where({
					$and: [
						{ slug: { $ne: this.slug } },
						{ tags: { $containsAny: this.tags } },
						{ date: { $lt: Date.now() } },
					],
				})
				.sortBy('published_at', 'desc')
				.limit(3)
				.fetch()
			if (this.relatedPosts.length < 3) {
				const morePosts = await this.$content(`blog`, { deep: true })
					.only(['title', 'slug'])
					.where({
						$and: [
							{
								slug: {
									$nin: [this.slug, ...this.relatedPosts.map((t) => t.slug)],
								},
							},
							{ category: { $in: this.tags.flat() } },
							{ date: { $lt: Date.now() } },
						],
					})
					.sortBy('published_at', 'desc')
					.limit(3 - this.relatedPosts.length)
					.fetch()
				this.relatedPosts = this.relatedPosts.concat(morePosts)
			}
		} catch (error) {}
	},
	data() {
		return {
			relatedPosts: {},
		}
	},
}
</script>
<style scoped>
section {
	@apply hidden;
	@apply lg:flex;
	@apply flex-col;
}

h3 {
	@apply mt-5;
}

li {
	@apply mx-2;
}

.related a {
	@apply text-gray-200;
}

.related a:hover {
	@apply text-pink-500;
}

li.link--active a {
	@apply text-pink-400;
	@apply dark:text-gray-50;
}
</style>
