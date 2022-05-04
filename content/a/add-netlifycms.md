---
date: 2022-04-18T17:00:29.149Z
title: "Theme plus: Add Netlify CMS to an existing site with Huguette"
introduction: |
  Having second thoughts? Adding NetlifyCMS later is not easy, but certainly possible!
---
## Adding Netlify CMS

I'm not joking when I say it's not easy, and really recommend you use the one-click install for a brand new site with Huguette, the css and NetlifyCMS enabled:

[![Deploy with Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/cathelijne/hugo-huguette-example&stack=cms)

But if you insist on adding Netlify CMS by hand, enable it from your config.toml. Add `netlifycms = true` to the params section so it looks like this:
```
[params]
  css = true
  netlifycms = true
```
Copy the static/admin folder to the static folder in the root of your site:
```
cp -r themes/huguette/static/admin static
```
You will need to edit config.yml in admin/static to match your site. Explaining how is outside of the scope if this installation doc, but you can use Netlify CMS's documentation: [instructions for adding NetlifyCMS](https://www.netlifycms.org/docs/hugo/) to Hugo.