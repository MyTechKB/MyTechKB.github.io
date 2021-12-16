---
title: "Git Commands"
date: 2021-12-14T21:23:08-06:00
draft: false
---

## Initialize global user
{{< highlight bash >}}
git config --global user.name "Your Name"
git config --global user.email "youremail@yourdomain.com"
{{< / highlight >}}

## Credentials stored with in ~/.git-credentials file
{{< highlight bash >}}
git config --global credential.helper store
{{< / highlight >}}

## Clone submodule
{{< highlight bash >}}
git submodule init
git submodule update
{{< / highlight >}}

## Remove submodule
{{< highlight bash >}}
mv yoursubmodule yoursubmodule_tmp
git submodule deinit yourSubmodule
git rm yourSubmodule
mv yoursubmodule_tmp yoursubmodule
git add yoursubmodule
{{< / highlight >}}
