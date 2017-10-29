# Other projects with static site generator

## 1. Pure static site with Netlify

_tested_

In this activity, we hardcode our site by ourself but we deploy and host the site with Netlify; so there nothing to build on the provider.

Pure static website : clone [this site](https://github.com/goffinet/crackciscotype7password) and/or [netlify it](https://app.netlify.com/start/deploy?repository=https://github.com/goffinet/crackciscotype7password) without any build command.

## 2. Gitbook Toolchain in Netlify

_summarily tested_

What is Gitbook ?

![](https://camo.githubusercontent.com/c1b6c55fca8e171120ce1fd73afcee699cc2a98f/68747470733a2f2f7261772e6769746875622e636f6d2f476974626f6f6b494f2f676974626f6f6b2f6d61737465722f707265766965772e706e67)

>GitBook is a command line tool (and Node.js library) for building beautiful books using GitHub/Git and Markdown (or AsciiDoc). Here is an example: [Learn Javascript](https://www.gitbook.com/book/GitBookIO/javascript).

>You can publish and host books easily online using [gitbook.com](https://www.gitbook.com). A desktop editor is [also available](https://www.gitbook.com/editor).

>Check out the [GitBook Community Slack Channel](https://slack.gitbook.com), Stay updated by following [@GitBookIO](https://twitter.com/GitBookIO) on Twitter or [GitBook](https://www.facebook.com/gitbookcom) on Facebook.

>Complete documentation is available at [toolchain.gitbook.com](http://toolchain.gitbook.com/).

[Netlify this](https://app.netlify.com/start/deploy?repository=https://github.com/goffinet/gitbooktest) gitbook projects.

Source : https://github.com/GitbookIO/gitbook and https://github.com/rubenoid/gitbooktest.

## 3. Netlify CMS

_summarily tested_

What is Netlify CMS ?

![](https://www.netlifycms.org/img/demo.gif)

>Netlify CMS is a Content Management System for static sites, allowing collaborators to create, edit, review, and publish content without writing code or dealing with version control. It brings the ease of WordPress-style editing to the simplicity and speed of static sites.

>At its core, Netlify CMS is an open-source React app that acts as a wrapper for the Git workflow, using the GitHub API. This provides many advantages, including:

>Fast, web-based UI: with rich-text editing, real-time preview, and drag-and-drop media uploads.

>* Platform agnostic: works with most static site generators.
>* Easy installation: add two files to your site and hook up the backend by including in your build process or linking to our CDN.
>* Modern authentication: using GitHub and JSON web tokens.
>* Flexible content types: specify an unlimited number of content types with custom fields.
>* Fully extensible: create custom-styled previews, UI widgets, and editor plugins.

Source : https://www.netlifycms.org/docs/intro/.

Take a test drive : Netlify CMS can run in any frontend web environment, but the quickest way to try it out is by running it on a pre-configured starter site with Netlify. this example here is the [Kaldi coffee company template](https://github.com/netlify-templates/one-click-hugo-cms) : Netlify [this project](https://app.netlify.com/start/deploy?repository=https://github.com/netlify-templates/one-click-hugo-cms&stack=cms) Netlify CMS and **enable github identity service in the netlify settings**. This site is running [Hugo static site generator](http://gohugo.io/).

Other Netlify templates are avaible here : https://github.com/netlify-templates.

## 4. Hosting sites with GitHub Pages

_tested_

Note : "gh-pages" = GitHub Pages

![](https://pages.github.com/images/slideshow/yeoman.png)

Hosting with GitHub Pages : https://pages.github.com/.

## 5. Webhooks with IFTT

_in project_

* Using Netlify Webhooks With IFTTT: https://www.jordanmerrick.com/posts/netlify-and-ifttt/ , what is [IFTTT](https://ifttt.com/) ?

## 6. Coding Modern Websites with the JAMstack

_in project_

Another example with [Hugo](http://gohugo.io/) and Netlify-CMS :

* https://www.netlify.com/blog/2016/11/15/new-to-jamstack-how-to-make-a-site-from-a-to-z/
* https://www.netlify.com/blog/2017/10/05/coding-modern-websites-with-the-jamstack-part-1/
* https://www.netlify.com/blog/2017/10/11/coding-modern-websites-with-the-jamstack-part-2/
* https://www.netlify.com/blog/2017/10/25/coding-modern-websites-with-the-jamstack-part-3/

## 7. Ghost Blog Self Hosting on Scaleway with Nginx, Cloudflare, and Let's Encrypt

_in dev_
