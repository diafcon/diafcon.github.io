---
title: "Setting Up docs app on local machine"
author: anslem
draft: false
date: 2022-11-11
tags:
  - First Issue
categories:
  - First Issue
---

## In this article, ill show you how to setup the diafcon docs website on your local machine.

**Note**

The website is made using [hugo](). Which is bascically a go framework

### Setting up environment

- Well use a simple mangement tool called [scoop](https://scoop.sh) to install hugo.

```bash
iwr -useb get.scoop.sh | iex
 
scoop install hugo-extended

```

- Usually `go` is required to run the hugo server, so download and install [go]().

- Installer should handle setting up the `env variables`.

- Restart Pc for all changes to work perfectly.

- Now that you have installed hugo, you can clone the repo to a desired location on your drive.

`cd REPO_LOCATION`

`code .`

- The above commands opens up vs code.

- Now that you have your editor open. Run app with `hugo server` and it should be served at port `localhost:1313`
