[![Deploy with Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/cathelijne/hugo-huguette-example&stack=cms)

# One-click Netlify install of Hugo, with the Huguette theme and Netlify CMS
This is the code for a full static Hugo website install on Netlify, with the [Huguette theme for Hugo](https://github.com/cathelijne/hugo-theme-huguette/).

![Huguette theme thumbnail](https://github.com/cathelijne/hugo-theme-huguette/blob/main/images/tn.png?raw=true)

## See it in action
Here's an [example site](https://huguette.netlify.app/) to see what Huguette looks like.

## About this project
[Netlify CMS](https://www.netlifycms.org/) is a great way to edit your static site. They have several templates for one-click installation of static site builders, but their Hugo one uses a pretty extensive theme (Victor Hugo. Points for the name! And it looks beautiful. But it was literally a bit too rich for my use-case). I build websites for fun and to learn, and I wanted a simple boilerplate theme to start with. Not exactly start from scratch, but close. So I wrote [Huguette](https://github.com/cathelijne/hugo-theme-huguette/).
I also wanted to include the CMS. _I_ might be comfortable enough to write Markdown, but not everyone I build sites for is, and to wean them off of their php-mysql-driven CMS's, something WYSIWYG-like was needed. And so I decided to split the theme into a theme-only repository and this full site-one (that includes the theme as a git submodule of course).

## Installation
Just click the button. Seriously. It's that easy. Or click [here](https://app.netlify.com/start/deploy?repository=https://github.com/cathelijne/hugo-huguette-example&stack=cms)

After clicking the button, authenticate with GitHub or GitLab and choose a repository name. Netlify then automatically creates a clone of the repository in your GitHub or GitLab account. Next, it builds and deploys the new site on Netlify, bringing you to the site dashboard after completing the build.

### Access Netlify CMS on your new site
The template deploy process sends you an invitation to your new site, sent from no-reply@netlify.com. The subject line looks like this: _You've been invited to join radiologist-amanda-53841.netlify.com_

1. Wait for the deployment to complete, then click the link to accept the invite. Your site will open with a prompt to create a password.
2. Enter a password, sign in, and you’ll go to the CMS. (For future visits, you can go straight to <yoursiteaddress.com>/admin/.)

Try adding and editing posts, or changing the content of the any page. When you save, the changes are pushed immediately to your Git repository, triggering a build on Netlify, and updating the content on your site. Check out the configuration code by visiting your site repo.

## I just want the theme, thanks
It's [here](https://github.com/cathelijne/hugo-theme-huguette/)

# Thanks
- [Hugo](https://gohugo.io)
- [Netlify CMS](https://www.netlifycms.org/)
- [classless.css](https://classless.de/)
- [Sharad's shortcodes for Netlify CMS](https://github.com/sharadcodes/hugo-shortcodes-netlify-cms)