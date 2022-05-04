---
date: 2022-04-18T17:01:17.818Z
title: "Theme only: just add the theme to my site"
introduction: How to install Huguette as your Hugo theme - with optional CSS
---
## Install Hugo
If you're complete new to building sites with Hugo, follow their [Quick Start](https://gohugo.io/getting-started/quick-start/) top get up and running fast.

## Add the theme as a git submodule
Installing Huguette works in the same way as installing the default theme from their docs:
```
cd quickstart
git init
git submodule add https://github.com/cathelijne/hugo-huguette-example.git themes/huguette
```
Enable the theme in your Hugo configuration:
```
echo 'theme = "huguette"
disableKinds = ["RSS", "taxonomy", "taxonomyTerm"]' >> config.toml
```
Your theme is now installed and functional. Remember that it's just HTML and nothing else, so it doesn't look particularly good.

## Enable the CSS (optional, but it does look good!)
To make Huguette as pretty as she is, copy the contents of the static/css folder in your theme directory to the static directory in the root of your site
```
mkdir static
cp -r themes/huguette/static/css static
```
Enable the css in your config.toml:
```
echo '[params]
  css = true' >> config.toml
```
And that's it!
