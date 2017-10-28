# Demo MkDocs Material

## 1. What are static site generators ?

**Practice** : Learn about [MkDocs](http://www.mkdocs.org/) and [Material for MkDocs](http://squidfunk.github.io/mkdocs-material/).

* MkDocs is a fast, simple and downright gorgeous static site generator that's geared towards building project documentation. Documentation source files are written in Markdown, and configured with a single YAML configuration file.
* Material is a theme for MkDocs. It is built using [Google's Material Design guidelines](https://material.io/guidelines/material-design/).

**Practice :** See the [advantages and the disadvantages](https://www.quora.com/What-are-the-pros-and-cons-of-using-static-site-generators) of [static website generators](https://www.staticgen.com/).

**Practice :** You can choose so many projects using [static site generator](https://www.staticgen.com/).


## 2. Connect to GitHub

>Git is a version control system for tracking changes in computer files and coordinating work on those files among multiple people. It is primarily used for source code management in software development, but it can be used to keep track of changes in any set of files. As a distributed revision control system it is aimed at speed,[9] data integrity,[10] and support for distributed, non-linear workflows.

> Git was created by Linus Torvalds in 2005 for development of the Linux kernel, with other kernel developers contributing to its initial development.

>As with most other distributed version control systems, and unlike most client–server systems, every Git directory on every computer is a full-fledged repository with complete history and full version tracking abilities, independent of network access or a central server.
> Git is free software distributed under the terms of the GNU General Public License version 2.

Source : https://en.wikipedia.org/wiki/Git

**Practice :** [Learn Git](https://try.github.io/) and GitHub.

* Create a GitHub user account.
* Connect to Github.
* Install `git` or `GitHub Desktop` localy.

## 3. Deploy this site with Netlify

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

Here is the best part, [Deploy this site with Netlify.](https://app.netlify.com/start/deploy?repository=https://github.com/goffinet/demo-mkdocs-material)

* Choose a repository name, for example : `mysite-dev`
* Click on "Save and deploy".

**Practice :** discover the Netlify interface and features.

## 4. DNS Service and settings

1. Get a domaine name (https://www.ovh.com/fr/domaines/) : for example, `example.com`
* Choose a DNS service (https://www.cloudflare.com/)
* Create a CNAME `mysite mysite-dev.netlify.com`

## 5. Setup a custom domain

1. Go to "mysite/settings/general"
* Click on the button "Change site name" : for example `mysite`
* Go to "Settings/Somain management/Domains"
* Click on the button "Add a custom domain" : `mysite.example.com`

## 6. Secure your site with HTTPS

1. Go to Settings/Domain management/HTTPS
* Verify DNS is configured correctly before enabling HTTPS : click on the button "Verify DNS Configuration".
* Provision a certificate for your domain and enable HTTPS : click on the button "provision a certificate for your domain and enable HTTPS".
* Click on "Force HTTPS" after the certificate generation.

## 7. Customize your site

* Clone localy the repository
* Add some content pages  written in Markdown.
* Configure the `mkdocs.yml` file.
* Commit and push your new code with `git`.

```bash
git clone https://github.com/myaccount/mysite-dev/
cd mysite-dev
vi docs/index.md
vi mkdocs.yml
git add *
git commit -alias
git push
```

## 8. Suggested actions

* Create a [Google Analytics](https://analytics.google.com/) a site with a following ID.
* Create a site in your [disqus](https://disqus.com/admin/) account.
* Register the site to [Google Search console](https://www.google.com/webmasters/tools/home?hl=fr&pli=1) and lauchn the site indexation.
