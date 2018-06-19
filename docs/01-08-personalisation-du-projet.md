# 8. Personnalisation du projet

## 1. Personnalisez votre site

**Pratique :** Révisez Git avec le cours en ligne https://try.github.io/ ou encore avec le livre en ligne avec https://git-scm.com/book/en/v2/.

**Pratique :** [Apprenez le langage Markdown](https://www.markdowntutorial.com/): Markdown est essentiellement une syntaxe pour un format de texte simple, facile à lire, qui est conçu pour être converti en HTML ([source](https://www.oreilly.com/ideas/static-site-generators)). La plupart des moteurs de blogs ont commencé à offrir un support pour Markdown, y compris Wordpress.

**Pratique :** Installez localement un outil de développement web qui offre un support du langage Markdown, comme [Sublime Text](http://www.sublimetext.com/), [Atom](https://atom. io/), [Visual Studio Code](https://code.visualstudio.com/), ou [Brackets](http://brackets.io/).

Localement, personnalisez votre site et déployez-le:

1. Cloner localement le "repository" `https://github.com/myaccount/monsite01/`.
2. Ajoutez des pages de contenu écrites dans Markdown dans le répertoire `docs/`.
3. Configurez le fichier `mkdocs.yml` et ajoutez la partie récapitulative.
4. Validez et appuyez sur votre nouveau code avec `git`.

```bash
git clone https://github.com/myaccount/monsite01/
cd monsite01
vi docs/index.md
vi mkdocs.yml
git add *
git commit -m "personnalisation de site"
git push
```

Veuillez revenir à votre interface Web Netlify pour vérifier votre build et le déploiement du site Web.

Note: Vous pouvez trouver de belles photos de qualité sur [Unsplash](https://unsplash.com/) (gratuit). Vous pouvez optimiser et transformer des images avec [Snappa](https://snappa.com/) (commercial), [CloudConvert](https://cloudconvert.com/) permet de convertir des fichiers notamment vers le format Markdown.

## 2. Aller plus loin

**Pratique :** Revoir [théorie des motifs MVC](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller), [concepts CSS](https: // fr .wikipedia.org / wiki / Cascading_Style_Sheets), [langage HTML](https://en.wikipedia.org/wiki/HTML) et [concepts SEO](https://en.wikipedia.org/wiki/Search_engine_optimization), Google Analytics, Google Search Consol, Woorank.

Allez plus loin avec vos nouvelles compétences:

1. Créez un ID de suivi [Google Analytics](https://analytics.google.com/).
2. Créez un site dans votre compte [disqus](https://disqus.com/admin/).
3. Enregistrez le site sur [Google Search Console](https://www.google.com/webmasters/tools/home?hl=fr&pli=1) et lancez l'indexation du site.
4. Créez un `docs/images/` pour stocker des images locales au site Web.
5. Intégrez un formulaire Mailchimp ou un widget Twitter, ou ajoutez un bloc de bannière AdSense.
6. [Modifier le thème MkDocs](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Themes) et/ou exploiter leur CSS.
7. Validez votre site avec [Woorank](https://www.woorank.com/).
