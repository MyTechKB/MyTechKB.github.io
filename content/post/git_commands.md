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
# Remove the submodule entry from .git/config
git submodule deinit -f path/to/submodule
# Remove the submodule directory from the superproject's .git/modules directory
rm -rf .git/modules/path/to/submodule
# Remove the entry in .gitmodules and remove the submodule directory located at path/to/submodule
git rm -f path/to/submodule
{{< / highlight >}}
