---
date: 2022-04-16T11:32:39.770Z
title: Enable Netlify CMS
introduction: >-
  The easiest way to use Netlify CMS with your Hugo site is to use Netlify to
  host your static site. Whenever you push to your Github repository, Netlify
  will automatically build and publish your site.


  Huguette has links to the Netlify part built-in (but will only include those in your static files if you enable Netlify CMS, see below). I highly recommend that you also copy the example site over to your site to have a few Netlify CMS catergories to start with.
---
## Preparing your files

Enable the inclusion of the CMS and the Netlify Identity checker by enabling it in your config.toml, like you did for the CSS:

```
[params]
  netlifycms = true
```

If you enabled the CSS in the previous step, there will already be a `params` section in your config.toml already. Make sure to add netlify to the same block. If you enabled both, the block will look like this:

```
[params]
  netlifycms = true
  css = true
```

## Connect Netlify to Github

Before you can connect Netlify and Github, push your site to github (run `git push` from the root of your site). Explaining how git and Github work is out of scope for this article, but if you need help with it Github's [Quickstart](https://docs.github.com/en/get-started/quickstart) is an excellent resource.

Next, log in to [Netlify](https://app.netlify.com) with your Github account.

![Login screen for https://app.netlify.com](/img/screenshot-2022-04-16-at-14.40.07.png)

![](/img/screenshot-2022-04-16-at-21.27.47.png)

![](/img/screenshot-2022-04-16-at-21.28.25.png)

![](/img/screenshot-2022-04-16-at-21.29.07.png)

TODO: check the stuff below with a NEW account and get screenshots/document better

* Sites -> Create new site
* Existing site
* From Github
* Follow the prompts to enable Netlify to access all or some of your github repos.

Now you can log on to https://yoursite/admin with your github credentials