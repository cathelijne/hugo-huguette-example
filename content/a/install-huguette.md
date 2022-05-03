---
date: 2022-04-18T17:00:17.818Z
title: Install Huguette
introduction: How to install Huguette as your Hugo theme
---
If you're complete new to building sites with Hugo, follow their [Quick Start](https://gohugo.io/getting-started/quick-start/) top get up and running fast.

Installing Huguette works in the same way as installing the default theme from their docs:

```
cd quickstart
git init
git submodule add https://github.com/cathelijne/hugo-huguette-example.git themes/huguette
```

Copy the contents of the static folder in your theme directory to the static directory in the root of your site

```
cp -r themes/huguette/static/ static
```

Enable the theme in your Hugo configuration:

```
echo 'theme = "huguette"
disableKinds = ["RSS", "taxonomy", "taxonomyTerm"]' >> config.toml
```

And that's it!
