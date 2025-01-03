---
layout: post
title: How to copy or move millions of files concurrently in linux
date: 2024-01-04 18:29:14 +0500
categories: [linux, backend story]
tags: [how to, linux, copy, files, move, concurrently, housekeeping] # TAG names should always be lowercase
featured: true
giscus_comments: true
---

Sometimes, you need to copy or move files from one drive to another. Copying or moving files using `cp` / `mv` one by one can take considerable time some times days and weeks depending upon number of files, size of individual file and disk speed.

Here's one way to speed up this process by using which you can copy / move millions of files concurrently from one directory to another in linux utilizing all CPU threads.

```
find . -type f | parallel --bar cp {} /path/to/destination
```

Break down of this command:

`find . -type f` means find all files in current directory. We then pipe this list to a tool called `parallel` which runs `cp` on all files in multithreaded fashion. `{}` is a placeholder for the current file to be copied to the destination folder, which is `/path/to/destination` in this case. And `--bar` is used to display a progress bar.

You might have to install `parallel` package (using `apt`, `pacman`, `dnf`, `yum` or whatever package manager your distro has) if its not already installed. Its available in all main line linux distros.

I learned this trick during my job as a backend developer. It can save you some time if you are trying to copy millions of large files from one drive to another. Sometimes, it can bring the copy / move time to hours from days and to days from weeks!
