---
layout: post
title: Are you sick of Youtube ads and clickbaity thumbnails?
date: 2025-04-20 22:17:31 +0500
categories: [free and open source software]
tags: [foss, life hacks, privacy, degoogle, tips, tricks, open source] # TAG names should always be lowercase
featured: true
giscus_comments: true
---

Youtube is one of the most used platform. I am sure you visit youtube.com or open Youtube app on your smartphone almost
every day. Youtube is a great video platform especially for learning and education but the business model of Youtube
and its parent company Google is not very privacy friendly.

Ad-revenue business model exploits user privacy for profit but this is a story for another day. In this article,
I will share some tricks that you can use to enhance your youtube experience by making it less intrusive and less clickbaity.
We all know that the Youtube's recommendation algorithm does its job very well. One click on suggested videos can take you away
from the purpose for which you had opened the site at first place.

# For Desktop

Use following extensions:

1. <a href='https://ublockorigin.com/' target='_blank'>uBlock Origin</a>: It is more than an ad blocker. Its a content blocker. With this extension installed your internet experience overall will become very friendly as uBlock will not allow ads on any site. Its truly amazing. Chrome users can install <a href='https://chromewebstore.google.com/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcphecmpfh?hl=en'> lite version of ublock origin </a>.
2. <a href='https://github.com/pietervanheijningen/clickbait-remover-for-youtube' target='_blank'> Clickbait remover </a>: This extension will liberate you from those clickbaity thumbnails that have weird red arrows and shapes to grab your attention. What this extension does is basically take a snaphot from start, middle or end of the video (you can customize this) and shows it as the thumbnail of video. Once you enable it and I am sure then you won't go back from this.
3. <a href='https://github.com/Vulpelo/hide-youtube-shorts' target='_blank'> Hide Youtube shorts</a>: Blocks youtube shorts from everywhere because lets agree shorts are not good for your mental health.
4. <a href='https://invidious.io/' target='_blank'>Invidious</a>: Invidious is basically a custom free and open source frontend for youtube. All videos on it are served through youtube servers directly but the information shown on home page and in search results is kind of based on web scraping techniques as it does not rely on official youtube api. It can run without Javascript which is a huge win for privacy.

# For Android

You can use youtube frontend clients like:

1. <a href='https://newpipe.net/' target='_blank'>Newpipe</a>: This is an open source app for android that lets you watch and download youtube videos for free. Also note that it does not require you to sign in with a google account to use it. This is a great win for privacy enthusiasts.
2. <a href='https://libretube.dev/' target='_blank'>Libretube</a>: Another open source app that you can use to browse youtube content on android for free. Libretube uses invidious.io as its backend api to extract, fetch and serve videos to its users. It has one added benefit over Newpipe that it won't reveal your IP address to google because it uses invidious as a proxy.

All of these extensions, youtube frontend clients and apps are free and open source. This means that neither do you have to pay for any of these amazing pieces of softwares nor do you have to pirate them. Additionally, open source means that these softwares have published their code for everyone to see and audit. Thus, you can use these softwares without any worry as they are legit and do not have any spyware or malware in them.

At the end, I am going to add a video walkthrough of Newpipe that will help you with installation and will also explain how to navigate Newpipe to have ad free youtube experience on your android smartphone.

<div class="row justify-content-sm-center">
    <a href="http://www.youtube.com/watch?feature=player_embedded&v=W3lFHnGP8Ow" target="_blank">
        <img src="http://img.youtube.com/vi/W3lFHnGP8Ow/0.jpg" alt="A guide on how to install and use Newpipe - an open source YT frontend" class="img-fluid rounded z-depth-1"/>    
    </a>
</div>
<div class='caption'>
A guide on how to install and use Newpipe - an open source YT frontend
</div>
