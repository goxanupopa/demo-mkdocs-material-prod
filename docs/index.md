# Continuous Deployment With Static Site Generators in Ten Steps

https://github.com/cd-static-gen/

English version. There is no French version.

## Summary

This document pursues the educational objective to learn continuous deployment with static site generators in ten steps :

1. What is continuous deployment ?
2. What is a static site generator ?
3. Connect to GitHub.
4. Deploy this site with Netlify.
5. Configure DNS Service and settings.
6. Setup a custom domain.
7. Secure your site with HTTPS.
8. Customize your site.
9. Suggested actions.
10. Other projects.

## 1. What is continuous deployment ?

Continuous deployment can be thought of as an extension of [continuous integration](https://www.agilealliance.org/glossary/continuous-integration/), aiming at minimizing [lead time](https://www.agilealliance.org/glossary/lead-time/), the time elapsed between development writing one new line of code and this new code being used by live users, in production.

Source : https://www.agilealliance.org/glossary/continuous-deployment/.

![](https://puppet.com/sites/default/files/2016-09/puppet_continuous_diagram.gif)

Source : https://puppet.com/blog/continuous-delivery-vs-continuous-deployment-what-s-diff.

## 2. What is a static site generator ?

> The basic concept of a static site generator (aka static site engine) is simple: take dynamic content and data and generate static HTML/JavaScript/CSS files that can be deployed to the server. This idea isn't new.

See this source : https://www.oreilly.com/ideas/static-site-generators.

* There are numerous services, both free and paid, that offer the ability to add dynamic aspects into static pages.
* Static site files are delivered to the end user exactly as they are on the server.
* There is no server-side language.
* There is no database.
* Static sites are HTML, CSS, and JavaScript.
* Performance, Hosting, Security, Content versioning are benefits of Static Sites.

**Practice** : Learn about [MkDocs](http://www.mkdocs.org/) and [Material for MkDocs](http://squidfunk.github.io/mkdocs-material/).

* MkDocs is a fast, simple and downright gorgeous static site generator that's geared towards building project documentation. Documentation source files are written in Markdown, and configured with a single YAML configuration file.
* Material is a theme for MkDocs. It is built using [Google's Material Design guidelines](https://material.io/guidelines/material-design/).

![](http://squidfunk.github.io/mkdocs-material/images/material.png)

**Practice :** You can choose so many projects using [static site generator](https://www.staticgen.com/).

## 3. Connect to GitHub

>Git is a version control system for tracking changes in computer files and coordinating work on those files among multiple people. It is primarily used for source code management in software development, but it can be used to keep track of changes in any set of files. As a distributed revision control system it is aimed at speed, data integrity, and support for distributed, non-linear workflows.

> Git was created by Linus Torvalds in 2005 for development of the Linux kernel, with other kernel developers contributing to its initial development.

>As with most other distributed version control systems, and unlike most client–server systems, every Git directory on every computer is a full-fledged repository with complete history and full version tracking abilities, independent of network access or a central server.

> Git is free software distributed under the terms of the GNU General Public License version 2.

Source : https://en.wikipedia.org/wiki/Git

**Practice :** [Learn Git](https://try.github.io/) and GitHub.

1. Create a GitHub user account.
2. Connect to Github.
3. Install [`git`](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) or [`GitHub Desktop`](https://help.github.com/desktop/guides/getting-started-with-github-desktop/installing-github-desktop/#platform-windows) localy.

## 4. Deploy this site with Netlify

**Practice :** [Learn what is Netlify (builds, deploys, and hosts websites in continous development mode)](https://www.netlify.com/docs/continuous-deployment/).

Netlify personal plan (free) features :

* Personal or commercial projects
* Public or private repositories
* HTTPS for custom domains
* Continuous Deployment
* Form handling (BETA)
* Community support
* Identity service (BETA)
* Split Testing (BETA)
* Git Gateway (BETA)

Source : https://www.netlify.com/pricing/

**Practice :** See what is a front end build tool like Grunt, Gulp or Broccoli.

* [Grunt](https://gruntjs.com/) : Why use a task runner?
In one word: automation. The less work you have to do when performing repetitive tasks like minification, compilation, unit testing, linting, etc, the easier your job becomes. After you've configured it through a Gruntfile, a task runner can do most of that mundane work for you—and your team—with basically zero effort.
* [Gulp](https://gulpjs.com/) : gulp is a toolkit for automating painful or time-consuming tasks in your development workflow, so you can stop messing around and build something.
* [Broccoli](https://github.com/broccolijs/broccoli) : A fast, reliable asset pipeline, supporting constant-time rebuilds and compact build definitions. Comparable to the Rails asset pipeline in scope, though it runs on Node and is backend-agnostic.

Deploy this site with Netlify :

1. Here is the best part, [Deploy this site with Netlify.](https://app.netlify.com/start/deploy?repository=https://github.com/goffinet/demo-mkdocs-material).
2. Choose a repository name, for example : `mysite-dev`.
3. Click on "Save and deploy".

**Practice :** discover the Netlify interface and features.

## 5. Configure  DNS Service and settings

**Practice :** Distinguish Domain Registrar service and DNS Service.

**Practice :** Review the [DNS concepts](https://en.wikipedia.org/wiki/Domain_Name_System).

**Practice :** Learn [what is cloudflare](https://blog.cloudflare.com/what-is-cloudflare/).

1. Get a domaine name (https://www.ovh.com/fr/domaines/) : for example, `example.com`.
2. Choose Cloudflare NS IP addresses.
3. Choose a DNS service (https://www.cloudflare.com/).
4. Create a CNAME `mysite mysite-dev.netlify.com`.

## 6. Setup a custom domain

Setup a custom domain :

1. Go to "mysite/settings/general".
2. Click on the button "Change site name" : for example `mysite`.
3. Go to "Settings/Somain management/Domains".
4. Click on the button "Add a custom domain" : `mysite.example.com`.

## 7. Secure your site with HTTPS

**Practice :** Review HTTPS security and certificates concepts.

**Practice :** Learn about [Let’s Encrypt](https://letsencrypt.org/about/). Let’s Encrypt is a free, automated, and open certificate authority (CA), run for the public’s benefit. It is a service provided by the [Internet Security Research Group (ISRG)](https://letsencrypt.org/isrg/).

Let’s Encrypt gives people the digital certificates they need in order to enable HTTPS (SSL/TLS) for websites, for free, in the most user-friendly way we can. We do this because we want to create a more secure and privacy-respecting Web.

Secure your site with HTTPS :

1. Go to Settings/Domain management/HTTPS.
2. Verify DNS is configured correctly before enabling HTTPS : click on the button "Verify DNS Configuration".
3. Provision a certificate for your domain and enable HTTPS : click on the button "provision a certificate for your domain and enable HTTPS".
4. Click on "Force HTTPS" after the certificate generation.

## 8. Customize your site

**Practice :** Review git with https://try.github.io/ or with https://git-scm.com/book/en/v2/.

**Practice :** [Learn the Markdown Language](https://www.markdowntutorial.com/) : Markdown is essentially a syntax for a simple, easy-to-read, plain text format that is designed to be converted to HTML ([source](https://www.oreilly.com/ideas/static-site-generators)). Most blog engines have started offering support for Markdown, including Wordpress.

**Practice :** Install localy a web-development tools that offers Markdown support out of the box, as [Sublime Text](http://www.sublimetext.com/), [Atom](https://atom.io/), [Visual Studio Code](https://code.visualstudio.com/), or [Brackets](http://brackets.io/).

Customize your site :

1. Clone localy the repository `https://github.com/myaccount/mysite-dev/`.
2. Add some content pages  written in Markdown into the `docs/` directory.
3. Configure the `mkdocs.yml` file and adat the summary part.
4. Commit and push your new code with `git`.

```bash
git clone https://github.com/myaccount/mysite-dev/
cd mysite-dev
vi docs/index.md
vi mkdocs.yml
git add *
git commit -m "site customization"
git push
```

## 9. Suggested actions

Suggested actions :

1. Create a [Google Analytics](https://analytics.google.com/) a site with a following ID.
2. Create a site in your [disqus account](https://disqus.com/admin/).
3. Register the site to [Google Search console](https://www.google.com/webmasters/tools/home?hl=fr&pli=1) and launch the site indexation.
4. Create a `docs/images/` to store pictures.
5. Integrate Mailchimp forms, ...

## 10. Other projects

### 10.1. Pure static site

Pure static website : clone [this site](https://github.com/goffinet/crackciscotype7password) and/or [netlify it](https://app.netlify.com/start/deploy?repository=https://github.com/goffinet/crackciscotype7password) without any build command.

### 10.2. Gitbook

What is Gitbook ?

![](https://camo.githubusercontent.com/c1b6c55fca8e171120ce1fd73afcee699cc2a98f/68747470733a2f2f7261772e6769746875622e636f6d2f476974626f6f6b494f2f676974626f6f6b2f6d61737465722f707265766965772e706e67)

>GitBook is a command line tool (and Node.js library) for building beautiful books using GitHub/Git and Markdown (or AsciiDoc). Here is an example: [Learn Javascript](https://www.gitbook.com/book/GitBookIO/javascript).

>You can publish and host books easily online using [gitbook.com](https://www.gitbook.com). A desktop editor is [also available](https://www.gitbook.com/editor).

>Check out the [GitBook Community Slack Channel](https://slack.gitbook.com), Stay updated by following [@GitBookIO](https://twitter.com/GitBookIO) on Twitter or [GitBook](https://www.facebook.com/gitbookcom) on Facebook.

>Complete documentation is available at [toolchain.gitbook.com](http://toolchain.gitbook.com/).

[Netlify this](https://app.netlify.com/start/deploy?repository=https://github.com/goffinet/gitbooktest) gitbook projects.

Source : https://github.com/GitbookIO/gitbook and https://github.com/rubenoid/gitbooktest.

### 10.3. Netlify-CMS

What is Netlify-CMS ?

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

Netlify [this project](https://app.netlify.com/start/deploy?repository=https://github.com/netlify-templates/one-click-hugo-cms&stack=cms) Netlify-CMS and **enable github identity service in the netlify settings**.

### 10.4. Hosting sites with gh-pages

![](https://pages.github.com/images/slideshow/yeoman.png)

Hosting with GitHub Pages : https://pages.github.com/.
