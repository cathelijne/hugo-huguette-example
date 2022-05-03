---
date: 2022-04-16T11:25:10.483Z
title: Enable the CSS
introduction: Enabling the CSS is as simple as adding it to your config.toml
---
Huguette looks at you site's parameters to see if it needs to enable the CSS.

Add the following lines *at the bottom* of your config.toml:

```
[params]
  netlifycms = false
  css = true
```

If you started with a fresh Hugo, there will be no `params` section in config.toml. But if there is, make sure that you do include `css = true` in that block and not accidentally create a new one.