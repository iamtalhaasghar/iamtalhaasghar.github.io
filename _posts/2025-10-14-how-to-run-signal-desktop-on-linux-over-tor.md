---
layout: post
title: How to run signal desktop over tor on laptop?
date: 2025-10-14 20:50:46 +0500
categories: [free and open source software]
tags: [foss, life hacks, privacy, degoogle, tips, tricks, open source] # TAG names should always be lowercase
featured: true
giscus_comments: true
---

Signal is one of the most secure and private messaging platform out there. So much so you that you will often hear Edwar Snowden
talking about it and recommending it from time to time. Even whatsapp's encryption algorithm is based on signal's Gold standard encryption protocol. This is exactly the reason why entities who might not want you to communicate securely or privately in a fashion that is very hard to evasedrop upon and might block or create hurdles in the ability to do so. Although signal mobile
app has built in circumvention capabilities but the signal desktop still lacks this very much needed feature.

So, in this guide how as a linux user you can bypass any geoblocking through tor for free so that when the time comes you are prepared to communicate in a secure fashion with your peers or friends.

# Step 1 - Install tor

This should be very straight forward. Depending upon your linux distro, use package manager of your choice and install tor package. Its available in almost all distro repos.

## arch

`pacman install tor`

## debian

`apt install tor`

## fedora

`dnf install tor`

Make sure it is running just fine with:
`systemctl status tor`

# Step 2 - Install Signal Desktop

Signal desktop can be installed very easily on debian based distros (ubuntu, mint, PopOS etc). Instructions are available on official signal website. Signal desktop package is also available in arch official repos. Fedora / Opensuse users can rely on the following repository to install signal desktop on their systems:

[https://software.opensuse.org/download.html?project=network:im:signal&package=signal-desktop](https://software.opensuse.org/download.html?project=network:im:signal&package=signal-desktop)

# Step 2 - Modify signal desktop application entry to route traffic through tor

So in this step what we are going to do is that we will use linuxs' enviornment variable and make sure that all traffic goes through tor's socks5 proxy port. This needs to be done before signal desktop is launched. We will automate it in a bit but you can test it out in a terminal using following command:

`env https_proxy=socks5://127.0.0.1:9050 signal-desktop -- %u`

The default port where tor service listens for sock5 proxy traffic is 9050. What we are doing with this command is essentially
telling signal desktop to use tor's sock5 proxy port 9050 for all incoming and outgoing connections. Thus, this makes signal desktop work like a charm.

# Step 3 - modify signal desktop applications entry

Now head over to `/usr/share/applications/signal-desktop.desktop` and modify the `Exec` paramater as following:
`Exec=env https_proxy=socks5://127.0.0.1:9050 signal-desktop -- %u`

With this what will happen is every time before you will run signal desktop automatically https_proxy will be injected and you won't have to do it manually.

# Step 4 - run signal desktop

Now run signal desktop from start menu and it should run just fine and you won't have to add env variable for socks5 again and again before running it.

Feel free to drop a comment if you have any queries or if you need any help. I will try to respond!
