---
layout: post
date: 2020-01-16 19:01
title: "Facial recognition on live video with JavaScript"
image: https://res.cloudinary.com/dk3rdh3yo/image/upload/w_auto,c_scale/73209458-e294bc00-410d-11ea-8ade-44d30e0b6cc3_okqk9n.png
description: "Adding facial recognition to an OpenTok video using Azure Face API"
comments: true
tags: [twitch, stream, opentok, azure, sentiment, face-api]
replay: https://youtu.be/5kCYw0qqiI8
---

### Stream Replay Link

[{{page.replay}}]({{page.replay}})

<!--more-->

### Segments

| Timestamp | Topic
| ---       | ---
| [00:44]({{page.replay}}?t=2669.259) | Kicking it off |
| [00:45]({{page.replay}}?t=2703.888) | I'm the king of the swingers yeah, jungle VIP |
| [00:45]({{page.replay}}?t=2728.982) | me James, I WILL become King |
| [02:51]({{page.replay}}?t=10306.166) | battle of the bat men |

### Today's Candle To Code By

<a href="https://stinkycandlecompany.com/product/wet-grass-candle" target="_blank">Wet Grass</a>

## Today's stream brought to you by

### Subscribers

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/fee37bef-5c1b-46e6-a1df-3b3f1d28b64d-profile_image-300x300.png"/>
    <span>RyannosaurusRex<br/>
      <a href="https://twitch.tv/ryannosaurusrex" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/7d5a92ba-8ac0-4731-b0d0-bd469342d146-profile_image-300x300.png"/>
    <span>JTsom<br/>
      <a href="https://twitch.tv/jtsom" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/8c8f1e74-7247-4418-8092-23addb6f452d-profile_image-300x300.png"/>
    <span>dot_commie<br/>
      <a href="https://twitch.tv/dot_commie" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>

### Cheers

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e0d81e861b461f14-profile_image-300x300.jpeg"/>
    <span>Wally_KC<br/>
      <a href="https://twitch.tv/wally_kc" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/73016bf4-5cc4-4d09-bed3-6db777c2e7e5-profile_image-300x300.png"/>
    <span>MarcusVoiceProgrammer<br/>
      <a href="https://twitch.tv/marcusvoiceprogrammer" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>

### Raids

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/2cc01832-4ccb-466a-8c76-e522e52cdf2b-profile_image-300x300.png"/>
    <span>Beachcasts<br/>
      <a href="https://twitch.tv/beachcasts" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>

### Moderators

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/20bd3f0a-ce68-4f5c-a9bf-f61b950be3d2-profile_image-300x300.png"/>
    <span>IAmNotMyself<br/>
      <a href="https://twitch.tv/iamnotmyself" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/notmyself" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/notmyself" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/b159c7c5-bbff-43d7-999a-7a0805f4893e-profile_image-300x300.jpg"/>
    <span>cmjchrisjones<br/>
      <a href="https://twitch.tv/cmjchrisjones" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/cmjchrisjones" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/cmjchrisjones" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e0b2472c-b103-44d3-b132-c618032217ef-profile_image-300x300.png"/>
    <span>RamblingGeek<br/>
      <a href="https://twitch.tv/ramblinggeek" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/rgeekuk" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/ramblinggeekuk" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/f7ff026e-98ca-4081-9e96-17e46b43df9d-profile_image-300x300.png"/>
    <span>phrakberg<br/>
      <a href="https://twitch.tv/phrakberg" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/solenberg" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/solenberg" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/abd243dc-3790-4a73-b7b4-1269f89ce083-profile_image-300x300.png"/>
    <span>parithon<br/>
      <a href="https://twitch.tv/parithon" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/0544659c-8d18-44dd-ae1b-b659553a4ffa-profile_image-300x300.jpg"/>
    <span>Clarkio<br/>
      <a href="https://twitch.tv/clarkio" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/_clarkio" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/clarkio" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
</div>

### Followers

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ce57700a-def9-11e9-842d-784f43822e80-profile_image-300x300.png"/>
    <span>theKushalGhosh<br/>
      <a href="https://twitch.tv/thekushalghosh" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/67f3c275-1c99-4bb9-aa6e-5db51b879329-profile_image-300x300.png"/>
    <span>YeahLater<br/>
      <a href="https://twitch.tv/yeahlater" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ebb84563-db81-4b9c-8940-64ed33ccfc7b-profile_image-300x300.png"/>
    <span>vikrend<br/>
      <a href="https://twitch.tv/vikrend" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/cdd517fe-def4-11e9-948e-784f43822e80-profile_image-300x300.png"/>
    <span>estrangedHD<br/>
      <a href="https://twitch.tv/estrangedhd" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/294c98b5-e34d-42cd-a8f0-140b72fba9b0-profile_image-300x300.png"/>
    <span>w4rp<br/>
      <a href="https://twitch.tv/w4rp" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ce57700a-def9-11e9-842d-784f43822e80-profile_image-300x300.png"/>
    <span>dnash126<br/>
      <a href="https://twitch.tv/dnash126" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>

### Contributors

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/20bd3f0a-ce68-4f5c-a9bf-f61b950be3d2-profile_image-300x300.png"/>
    <span>IAmNotMyself<br/>
      <a href="https://twitch.tv/iamnotmyself" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/notmyself" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/notmyself" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e0b2472c-b103-44d3-b132-c618032217ef-profile_image-300x300.png"/>
    <span>RamblingGeek<br/>
      <a href="https://twitch.tv/ramblinggeek" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/rgeekuk" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/ramblinggeekuk" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/3bdd5c96-e43c-4745-b3fc-d969f8f55121-profile_image-300x300.jpeg"/>
    <span>FBoucheros<br/>
      <a href="https://twitch.tv/fboucheros" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e270ed68-0556-4e4d-a96a-fe1a611fe520-profile_image-300x300.jpeg"/>
    <span>kidqueb<br/>
      <a href="https://twitch.tv/kidqueb" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/b159c7c5-bbff-43d7-999a-7a0805f4893e-profile_image-300x300.jpg"/>
    <span>cmjchrisjones<br/>
      <a href="https://twitch.tv/cmjchrisjones" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/cmjchrisjones" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/cmjchrisjones" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/9c9ed3b2-3ecb-4ada-b4bd-cdea50ce7044-profile_image-300x300.png"/>
    <span>SurlyDev<br/>
      <a href="https://twitch.tv/surlydev" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/73016bf4-5cc4-4d09-bed3-6db777c2e7e5-profile_image-300x300.png"/>
    <span>MarcusVoiceProgrammer<br/>
      <a href="https://twitch.tv/marcusvoiceprogrammer" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/f7ff026e-98ca-4081-9e96-17e46b43df9d-profile_image-300x300.png"/>
    <span>phrakberg<br/>
      <a href="https://twitch.tv/phrakberg" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/solenberg" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/solenberg" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/926c0d6b-bc04-4dba-88a6-915dc6c6bb54-profile_image-300x300.png"/>
    <span>CopperBeardy<br/>
      <a href="https://twitch.tv/copperbeardy" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/copperbeardy" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/copperbeardy" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/0b21b9c4-d5ac-4837-ba3f-35c4934ceef6-profile_image-300x300.png"/>
    <span>BrettMillerIT<br/>
      <a href="https://twitch.tv/brettmillerit" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/brettmiller_it" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/brettmillerb" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/abd243dc-3790-4a73-b7b4-1269f89ce083-profile_image-300x300.png"/>
    <span>parithon<br/>
      <a href="https://twitch.tv/parithon" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/fee37bef-5c1b-46e6-a1df-3b3f1d28b64d-profile_image-300x300.png"/>
    <span>RyannosaurusRex<br/>
      <a href="https://twitch.tv/ryannosaurusrex" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/b56b492c-4409-4dcb-9ed8-6391f368b50b-profile_image-300x300.jpg"/>
    <span>jam3sn_<br/>
      <a href="https://twitch.tv/jam3sn_" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/63a1ab96-e388-4937-8ae2-958aea48b799-profile_image-300x300.jpeg"/>
    <span>fishingdev<br/>
      <a href="https://twitch.tv/fishingdev" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/5c68c507-5498-44f4-a6c9-365902e28d0b-profile_image-300x300.png"/>
    <span>codephobia<br/>
      <a href="https://twitch.tv/codephobia" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/codephobia" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/codephobia" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/f43c0fb3-e87e-459d-b093-ef9393d874e5-profile_image-300x300.png"/>
    <span>MusicalBookworm<br/>
      <a href="https://twitch.tv/musicalbookworm" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ce57700a-def9-11e9-842d-784f43822e80-profile_image-300x300.png"/>
    <span>EternalDevCoder<br/>
      <a href="https://twitch.tv/eternaldevcoder" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/bfd92059-385a-44f5-8c50-c07ddd553e1c-profile_image-300x300.png"/>
    <span>SausageCam<br/>
      <a href="https://twitch.tv/sausagecam" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e0d81e861b461f14-profile_image-300x300.jpeg"/>
    <span>Wally_KC<br/>
      <a href="https://twitch.tv/wally_kc" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/13e5fa74-defa-11e9-809c-784f43822e80-profile_image-300x300.png"/>
    <span>jaronstrypsteen<br/>
      <a href="https://twitch.tv/jaronstrypsteen" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ebe4cd89-b4f4-4cd9-adac-2f30151b4209-profile_image-300x300.png"/>
    <span>h0usebesuch<br/>
      <a href="https://twitch.tv/h0usebesuch" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/kershoc-profile_image-be83643ea5351531-300x300.png"/>
    <span>Kershoc<br/>
      <a href="https://twitch.tv/kershoc" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/2cc01832-4ccb-466a-8c76-e522e52cdf2b-profile_image-300x300.png"/>
    <span>Beachcasts<br/>
      <a href="https://twitch.tv/beachcasts" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/angryapplegw2-profile_image-f548b26ed7650711-300x300.jpeg"/>
    <span>Angryapplegw2<br/>
      <a href="https://twitch.tv/angryapplegw2" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/9781a06c-3011-4a72-86e9-cdd1d8787e5d-profile_image-300x300.jpg"/>
    <span>ReturnToDust<br/>
      <a href="https://twitch.tv/returntodust" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/998f01ae-def8-11e9-b95c-784f43822e80-profile_image-300x300.png"/>
    <span>cloudhawke13<br/>
      <a href="https://twitch.tv/cloudhawke13" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/dd6f2848-b20e-4dc8-a90d-823abaf53034-profile_image-300x300.png"/>
    <span>sadmoody<br/>
      <a href="https://twitch.tv/sadmoody" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/7d5a92ba-8ac0-4731-b0d0-bd469342d146-profile_image-300x300.png"/>
    <span>JTsom<br/>
      <a href="https://twitch.tv/jtsom" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/d5068df5265f12b0-profile_image-300x300.png"/>
    <span>RobinMalfait<br/>
      <a href="https://twitch.tv/robinmalfait" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/dbdc9198-def8-11e9-8681-784f43822e80-profile_image-300x300.png"/>
    <span>giusdp<br/>
      <a href="https://twitch.tv/giusdp" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/0544659c-8d18-44dd-ae1b-b659553a4ffa-profile_image-300x300.jpg"/>
    <span>Clarkio<br/>
      <a href="https://twitch.tv/clarkio" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/_clarkio" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/clarkio" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/fa425591-26cb-49e5-9f6d-699b32038f55-profile_image-300x300.jpg"/>
    <span>ashishsinghbaghel<br/>
      <a href="https://twitch.tv/ashishsinghbaghel" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://github.com/mechdeveloper" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/f46f0100-fd8a-48ee-9f80-d43f34d58e3f-profile_image-300x300.jpeg"/>
    <span>AidanLynge<br/>
      <a href="https://twitch.tv/aidanlynge" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/72c4ef86-00a5-4124-b0c3-d5f51e5a22c9-profile_image-300x300.png"/>
    <span>BraveCobra2<br/>
      <a href="https://twitch.tv/bravecobra2" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/19ec13af-bf20-48bc-9d89-ba6c527c580f-profile_image-300x300.png"/>
    <span>JonathanDelfraisse<br/>
      <a href="https://twitch.tv/jonathandelfraisse" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/998f01ae-def8-11e9-b95c-784f43822e80-profile_image-300x300.png"/>
    <span>CodingStocks<br/>
      <a href="https://twitch.tv/codingstocks" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/998f01ae-def8-11e9-b95c-784f43822e80-profile_image-300x300.png"/>
    <span>bl3nd865<br/>
      <a href="https://twitch.tv/bl3nd865" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/c04137e8-b3af-412e-a826-6a08709e8335-profile_image-300x300.png"/>
    <span>LewHgh<br/>
      <a href="https://twitch.tv/lewhgh" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/lewhgh" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/lewhgh" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/d21cb3b8-6967-448d-a540-d0bd902afbe8-profile_image-300x300.png"/>
    <span>mindtrixz<br/>
      <a href="https://twitch.tv/mindtrixz" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>
