---
layout: post
date: 2019-11-17 18:11
title: "Putting our chat bot services in containers and testing in Azure."
image: https://user-images.githubusercontent.com/1228996/69594539-4988de00-0fc2-11ea-8829-81414b4a7af9.png
description: "Now that we have some Node.js apps, we put them in containers so we can run them in Azure."
comments: true
tags: [twitch, stream, vulcan, containers, azure]
replay: https://youtu.be/eN1uGfL5lZE
---

### Stream Replay Link

[{{page.replay}}]({{page.replay}})

<!--more-->

### Today's Candle To Code By

<a href="https://amzn.to/2GSsMxX" target="_blank">Warm Tobacco Pipe</a>

## Today's stream brought to you by

### Subscribers

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/294c98b5-e34d-42cd-a8f0-140b72fba9b0-profile_image-300x300.png"/>
    <span>Krennan<br/>
      <a href="https://twitch.tv/krennan" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/3d87767dfbf36816-profile_image-300x300.jpeg"/>
    <span>DoctorArgus<br/>
      <a href="https://twitch.tv/doctorargus" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>

### Cheers

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/romerocesar-profile_image-653a04e399c7e345-300x300.jpeg"/>
    <span>RomeroCesar<br/>
      <a href="https://twitch.tv/romerocesar" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/romerocesar-profile_image-653a04e399c7e345-300x300.jpeg"/>
    <span>RomeroCesar<br/>
      <a href="https://twitch.tv/romerocesar" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
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
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e0b2472c-b103-44d3-b132-c618032217ef-profile_image-300x300.png"/>
    <span>RamblingGeek<br/>
      <a href="https://twitch.tv/ramblinggeek" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/rgeekuk" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/ramblinggeekuk" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/b159c7c5-bbff-43d7-999a-7a0805f4893e-profile_image-300x300.jpg"/>
    <span>cmjchrisjones<br/>
      <a href="https://twitch.tv/cmjchrisjones" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/cmjchrisjones" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/cmjchrisjones" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/abd243dc-3790-4a73-b7b4-1269f89ce083-profile_image-300x300.png"/>
    <span>parithon<br/>
      <a href="https://twitch.tv/parithon" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/0544659c-8d18-44dd-ae1b-b659553a4ffa-profile_image-300x300.jpg"/>
    <span>Clarkio<br/>
      <a href="https://twitch.tv/clarkio" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>

### Followers

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/75305d54-c7cc-40d1-bb9c-91fbe85943c7-profile_image-300x300.png"/>
    <span>user135711<br/>
      <a href="https://twitch.tv/user135711" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ead5c8b2-a4c9-4724-b1dd-9f00b46cbd3d-profile_image-300x300.png"/>
    <span>tevieb<br/>
      <a href="https://twitch.tv/tevieb" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/41780b5a-def8-11e9-94d9-784f43822e80-profile_image-300x300.png"/>
    <span>abdenbiworks<br/>
      <a href="https://twitch.tv/abdenbiworks" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/41780b5a-def8-11e9-94d9-784f43822e80-profile_image-300x300.png"/>
    <span>juanecoperu<br/>
      <a href="https://twitch.tv/juanecoperu" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/2a99433c-9dc1-4640-aba7-e10891a9dcc2-profile_image-300x300.png"/>
    <span>Git_R_Done_77<br/>
      <a href="https://twitch.tv/git_r_done_77" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/romerocesar-profile_image-653a04e399c7e345-300x300.jpeg"/>
    <span>RomeroCesar<br/>
      <a href="https://twitch.tv/romerocesar" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>

### Contributors

<div class="users">
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/b159c7c5-bbff-43d7-999a-7a0805f4893e-profile_image-300x300.jpg"/>
    <span>cmjchrisjones<br/>
      <a href="https://twitch.tv/cmjchrisjones" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/cmjchrisjones" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/cmjchrisjones" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/294c98b5-e34d-42cd-a8f0-140b72fba9b0-profile_image-300x300.png"/>
    <span>darkysharky<br/>
      <a href="https://twitch.tv/darkysharky" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/8ccda334-10f3-4fb6-9756-417fe293ac48-profile_image-300x300.png"/>
    <span>ValentinMaziev<br/>
      <a href="https://twitch.tv/valentinmaziev" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ebe4cd89-b4f4-4cd9-adac-2f30151b4209-profile_image-300x300.png"/>
    <span>ChanceDev<br/>
      <a href="https://twitch.tv/chancedev" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/49134312-c13a-439d-b230-c7244d303d13-profile_image-300x300.png"/>
    <span>mrBalrog<br/>
      <a href="https://twitch.tv/mrbalrog" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/cd60b68d-824e-4e41-b7bb-8d9fb85258a7-profile_image-300x300.png"/>
    <span>fork04_<br/>
      <a href="https://twitch.tv/fork04_" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ead5c8b2-a4c9-4724-b1dd-9f00b46cbd3d-profile_image-300x300.png"/>
    <span>ecomath328<br/>
      <a href="https://twitch.tv/ecomath328" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/f43c0fb3-e87e-459d-b093-ef9393d874e5-profile_image-300x300.png"/>
    <span>MusicalBookworm<br/>
      <a href="https://twitch.tv/musicalbookworm" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e0b2472c-b103-44d3-b132-c618032217ef-profile_image-300x300.png"/>
    <span>RamblingGeek<br/>
      <a href="https://twitch.tv/ramblinggeek" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/rgeekuk" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/ramblinggeekuk" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/abd243dc-3790-4a73-b7b4-1269f89ce083-profile_image-300x300.png"/>
    <span>parithon<br/>
      <a href="https://twitch.tv/parithon" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/aaec869d-52c4-45ee-8300-d78d41d62b2b-profile_image-300x300.jpg"/>
    <span>Fihen<br/>
      <a href="https://twitch.tv/fihen" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/958a22b1-e9e5-4390-8843-98d9def72a35-profile_image-300x300.png"/>
    <span>sorskoot<br/>
      <a href="https://twitch.tv/sorskoot" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/sorskoot" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/sorskoot" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/75305d54-c7cc-40d1-bb9c-91fbe85943c7-profile_image-300x300.png"/>
    <span>FuleSnabel<br/>
      <a href="https://twitch.tv/fulesnabel" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/0b21b9c4-d5ac-4837-ba3f-35c4934ceef6-profile_image-300x300.png"/>
    <span>BrettMillerIT<br/>
      <a href="https://twitch.tv/brettmillerit" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/brettmiller_it" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/brettmillerb" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/926c0d6b-bc04-4dba-88a6-915dc6c6bb54-profile_image-300x300.png"/>
    <span>CopperBeardy<br/>
      <a href="https://twitch.tv/copperbeardy" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a><a href="https://twitter.com/copperbeardy" target="_blank"><i class="fab fa-twitter" aria-hidden="true"></i></a><a href="https://github.com/copperbeardy" target="_blank"><i class="fab fa-github" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/3d87767dfbf36816-profile_image-300x300.jpeg"/>
    <span>DoctorArgus<br/>
      <a href="https://twitch.tv/doctorargus" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/2cc01832-4ccb-466a-8c76-e522e52cdf2b-profile_image-300x300.png"/>
    <span>Beachcasts<br/>
      <a href="https://twitch.tv/beachcasts" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/998f01ae-def8-11e9-b95c-784f43822e80-profile_image-300x300.png"/>
    <span>bl3nd865<br/>
      <a href="https://twitch.tv/bl3nd865" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ce57700a-def9-11e9-842d-784f43822e80-profile_image-300x300.png"/>
    <span>orenong_live3<br/>
      <a href="https://twitch.tv/orenong_live3" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/nubium-profile_image-234628f6b3f101af-300x300.jpeg"/>
    <span>Nubium<br/>
      <a href="https://twitch.tv/nubium" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/0544659c-8d18-44dd-ae1b-b659553a4ffa-profile_image-300x300.jpg"/>
    <span>Clarkio<br/>
      <a href="https://twitch.tv/clarkio" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/ebb84563-db81-4b9c-8940-64ed33ccfc7b-profile_image-300x300.png"/>
    <span>davi2102<br/>
      <a href="https://twitch.tv/davi2102" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/75305d54-c7cc-40d1-bb9c-91fbe85943c7-profile_image-300x300.png"/>
    <span>user135711<br/>
      <a href="https://twitch.tv/user135711" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/d898b9a4-70fc-4eea-97ed-9c4a8cd8c1c8-profile_image-300x300.png"/>
    <span>SilvanoGJr<br/>
      <a href="https://twitch.tv/silvanogjr" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures/4cbf10f1-bb9f-4f57-90e1-15bf06cfe6f5-profile_image-300x300.jpg"/>
    <span>ceykil<br/>
      <a href="https://twitch.tv/ceykil" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/8885552c-74b0-4120-a6e4-1fd78eb87b0d-profile_image-300x300.png"/>
    <span>haydennyyy<br/>
      <a href="https://twitch.tv/haydennyyy" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/44ccf150-927c-4340-8a2b-582e5073c403-profile_image-300x300.jpg"/>
    <span>Kyruski<br/>
      <a href="https://twitch.tv/kyruski" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/user-default-pictures-uv/41780b5a-def8-11e9-94d9-784f43822e80-profile_image-300x300.png"/>
    <span>abdenbiworks<br/>
      <a href="https://twitch.tv/abdenbiworks" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/e61f8807-9429-4965-b988-627b54347695-profile_image-300x300.png"/>
    <span>lv2lrn4lf<br/>
      <a href="https://twitch.tv/lv2lrn4lf" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
  <div class="user">
    <img class="profile" src="https://static-cdn.jtvnw.net/jtv_user_pictures/romerocesar-profile_image-653a04e399c7e345-300x300.jpeg"/>
    <span>RomeroCesar<br/>
      <a href="https://twitch.tv/romerocesar" target="_blank"><i class="fab fa-twitch" aria-hidden="true"></i></a></span>
  </div>
</div>