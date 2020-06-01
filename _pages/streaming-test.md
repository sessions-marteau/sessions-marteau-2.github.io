---
layout: page
title: Streaming Test
image: 
permalink: /streaming-test/
tag: 
---

This is a streaming test.

<center>
<!-- Add a placeholder for the Twitch embed -->
<div id="twitch-embed"></div>

<!-- Load the Twitch embed script -->
<script src="https://embed.twitch.tv/embed/v1.js"></script>

<!-- Create a Twitch.Embed object that will render within the "twitch-embed" root element. -->
<script type="text/javascript">
  new Twitch.Embed("twitch-embed", {
    width: 1080,
    height: 480,
    channel: "eighthradio",
    // only needed if your site is also embedded on embed.example.com and othersite.example.com 
    // parent: ["embed.example.com", "othersite.example.com"]
  });
</script>

<center>
  
  
  test #2 no comment section and smaller for mobile 
  
  <iframe
    src="https://player.twitch.tv/?channel=eighthradio&parent=streamernews.example.com&muted=false"
    height="360"
    width="720"
    frameborder="0"
    scrolling="no"
    playsinline="true"
    allowfullscreen="true">
</iframe>

FB comments test
<div id="fb-root"></div>
<script async defer crossorigin="anonymous" src="https://connect.facebook.net/fr_CA/sdk.js#xfbml=1&version=v7.0&appId=238569848365&autoLogAppEvents=1"></script>

<div class="fb-comments" data-href="https://sessionsmarteau.com/streaming-test/" data-numposts="99" data-width=""></div>

