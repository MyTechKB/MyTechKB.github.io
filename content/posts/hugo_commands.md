---
title: "Hugo Commands"
date: 2021-12-12T21:58:14-06:00
draft: true
category: Quick Starts
tags:
- Blogging
- Hugo
---

# Hugo Commands

## Create a new site
{{< highlight bash >}}
hugo new site quickstart
{{< / highlight >}}

## Add a theme
[Hugo Themes](https://themes.gohugo.io/)
{{< highlight bash >}}
cd quickstart
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
{{< / highlight >}}

## Add some content
{{< highlight bash >}}
hugo new posts/my-first-post.md
{{< / highlight >}}

## Start the Hugo Server
{{< highlight bash >}}
hugo server -D
{{< / highlight >}}

## Site Configuration
Open up config.toml in a text editor

## Build static pages
{{< highlight bash >}}
hugo -D
{{< / highlight >}}

## Code Highlighting
{{< highlight bash >}}
\{\{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}"
// ... code
\{\{< / highlight >}}"
{{< / highlight >}}
