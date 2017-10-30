# Premier projet de déploiement continu

## Introduction

Dans ce cours, nous apprendrons comment déployer des sites Web en déploiement continu avec des générateurs de sites statiques. Nous essaierons de comprendre de nombreux concepts et de les mettre en pratique :

1. Planifiez votre projet.
2. Qu'est-ce qu'un déploiement continu?
3. Qu'est-ce qu'un générateur de site statique?
4. Connectez-vous à GitHub.
5. Déployez ce site avec Netlify.
6. Configurez le service DNS et les paramètres DNS.
7. Configurez un domaine personnalisé.
8. Sécurisez votre site avec HTTPS.
9. Personnalisez votre site.
10. Aller plus loin avec les générateurs de site statique.

Pour maintenir notre site, nous utiliserons **Git**, **GitHub** et **Atom Editor**.

Pour construire, déployer et héberger nos exemples, nous utiliserons **Netlify**.

Nous utiliserons **MkDocs**, **Hugo**, **GitBook** et **Jekyll** comme générateurs de sites statiques.

Il n'y a rien à payer pour utiliser et déployer ces solutions.

L'exemple principal tente de répondre au besoin d'un système de documentation Web à monter en 10 étapes.

Après cette première procédure, à la page suivante, nous étendrons nos connaissances avec d'autres projets.

## 1. Planifiez votre projet

Pour ce premier exemple, nous utiliserons ce plan :

Caractéristique | La description
--- | ---
Générateur statique | MkDocs
Thème | mkdocs-material
Type | Documentation
Nom | learn-cd-staticgen
Dépôt original | https://github.com/goffinet/learn-cd-staticgen/
Mon "repository" de projets | https://github.com/goffinet/learn-cd-staticgen-mkdocs-material-01/
Titre | Apprenez le déploiement continu avec des générateurs de site statiques en dix étapes
Description | Apprenez le déploiement continu avec des générateurs de site statiques en dix étapes
URL | https://learn-cd-staticgen.goffinet.org
Caractéristiques du site Web | Couleurs, contenu, structure, images, liens de liens sociaux, ...
Fournisseur de service CD | Netlify
DNS Registrar | OVH
Service DNS | Cloudflare sans proxy

Veuillez remplir votre premier plan personnel:

Caractéristique | La description
--- | ---
Générateur statique | MkDocs
Thème | mkdocs-material
Type | Documentation
Nom | learn-cd-staticgen ...
Dépôt original | https://github.com/goffinet/learn-cd-staticgen/
Mon "repository" de projets | https://github.com/.../...
Titre | ...
Description | ...
URL | https://...
Caractéristiques du site Web | Couleurs, contenu, structure, images, liens de liens sociaux, ...
Fournisseur de service CD | Netlify
DNS Registrar | ...
Service DNS | ...

## 2. Qu'est-ce qu'un déploiement continu?

Le déploiement continu peut être considéré comme une extension de [l'intégration continue](https://www.agilealliance.org/glossary/continuous-integration/), visant à minimiser [délai d'exécution](https://www.agilealliance.org/glossary/lead-time/), le temps écoulé entre le développement d'une nouvelle ligne de code et l'utilisation de ce nouveau code par les utilisateurs en production.

Source: https://www.agilealliance.org/glossary/continuous-deployment/.

![](https://puppet.com/sites/default/files/2016-09/puppet_continuous_diagram.gif)

Source: https://puppet.com/blog/continuous-delivery-vs-continuous-deployment-what-s-diff.

## 3. Qu'est-ce qu'un générateur de site statique?

> Le concept de base d'un générateur de site statique (aussi appelé moteur de site statique) est simple: prendre du contenu et des données dynamiques et générer des fichiers HTML/JavaScript/CSS statiques pouvant être déployés sur le serveur. Cette idée n'est pas nouvelle.

Voir cette excellente source: https://www.oreilly.com/ideas/static-site-generators.

* Il existe de nombreux services, gratuits et payants, qui offrent la possibilité d'ajouter des aspects dynamiques dans des pages statiques.
* Les fichiers de sites statiques sont livrés à l'utilisateur final exactement comme ils sont sur le serveur.
* Il n'y a pas de langage côté serveur.
* Il n'y a pas de base de données.
* Les sites statiques sont en HTML, CSS et JavaScript.
* Les performances, l'hébergement, la sécurité, la gestion des versions de contenu sont des avantages des sites statiques.

**Pratique**: En savoir plus sur [MkDocs](http://www.mkdocs.org/) et [Material for MkDocs](http://squidfunk.github.io/mkdocs-material/).

* MkDocs est un générateur de site statique rapide, simple et carrément magnifique qui est orienté vers la création de documentation de projet. Les fichiers sources de documentation sont écrits dans Markdown et configurés avec un seul fichier de configuration YAML.
* Le matériel est un thème pour MkDocs. Il est construit en utilisant [les directives de Google Material Design](https://material.io/guidelines/material-design/).

![](http://squidfunk.github.io/mkdocs-material/images/material.png)

**Pratique :** Vous pouvez choisir autant de projets à partir de [static site generator](https://www.staticgen.com/). N'hésitez pas à explorer staticgen.com.

## 4. Connectez-vous à GitHub

Qu'est-ce que Git ?

> Git est un système de contrôle de version pour suivre les changements dans les fichiers informatiques et coordonner le travail sur ces fichiers entre plusieurs personnes. Il est principalement utilisé pour la gestion de code source dans le développement de logiciels, mais il peut être utilisé pour suivre les changements dans n'importe quel ensemble de fichiers. En tant que système de contrôle de révision distribué, il vise la vitesse, l'intégrité des données et la prise en charge de flux de travail distribués et non linéaires.

> Git a été créé par Linus Torvalds en 2005 pour le développement du noyau Linux, avec d'autres développeurs du noyau contribuant à son développement initial.

> Comme avec la plupart des autres systèmes de contrôle de version distribués, et contrairement à la plupart des systèmes client-serveur, chaque répertoire Git de chaque ordinateur est un "repository" à part entière avec un historique complet et des capacités de suivi de version complètes.

> Git est un logiciel libre distribué sous les termes de la GNU General Public License version 2.

Source: https://en.wikipedia.org/wiki/Git

Qu'est-ce que GitHub ?

> GitHub est un "repository" Git ou de contrôle de version basé Web et un service d'hébergement Internet. Il est principalement utilisé pour héberger du code. Il offre toutes les fonctionnalités distribuées de contrôle de version et de gestion de code source (SCM, _source code management_) de Git, ainsi que l'ajout de ses propres fonctionnalités. Il fournit un contrôle d'accès et plusieurs fonctionnalités de collaboration telles que le suivi des bogues, les demandes de fonctionnalités, la gestion des tâches et les wikis pour chaque projet.

> Depuis avril 2017, GitHub compte près de 20 millions d'utilisateurs et 57 millions de dépôts, ce qui en fait la plus grande source de code source au monde.

> GitHub a une mascotte appelée Octocat, un chat avec cinq tentacules et un visage humain.

Source: https://en.wikipedia.org/wiki/GitHub

**Pratique :** [Learn Git](https://try.github.io/) et GitHub.

1. Créez un compte utilisateur GitHub.
2. Connectez-vous à Github.
3. Installez le logiciel [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) ou le logiciel [` GitHub Desktop`](https://help.github.com / desktop / guides / mise-en-marche-avec-github-desktop / installation-github-desktop / # plateforme-windows) localy.

## 5. Déployez ce site avec Netlify

**Pratique :** [En savoir plus sur Netlify (crée, déploie et héberge des sites Web en mode de développement continu)](https://www.netlify.com/docs/continuous-deployment/).

Fonctionnalités du plan personnel Netlify (gratuit):

* Projets personnels ou commerciaux
* Dépôts publics ou privés
* HTTPS pour les domaines personnalisés
* Déploiement continu
* Soutien communautaire
* Manipulation de formulaire (BETA)
* Service d'identité (BETA)
* Test de Split (BETA)
* Passerelle Git (BETA)

Source: https://www.netlify.com/pricing/

**Pratique :** Voir ce qu'est un "front end build tool" comme [Grunt](https://gruntjs.com/), [Gulp](https://gulpjs.com/) ou [Broccoli](https://github.com/broccolijs/broccoli) : des programmes d'exécution de tâches répétitives telles que minification, la compilation, les tests unitaires, etc.

Déployez ce site avec Netlify:

1. Voici la meilleure partie, [Déployez ce site avec Netlify](https://app.netlify.com/start/deploy?repository=https://github.com/goffinet/demo-mkdocs-material).
2. Choisissez un nom de "repository", par exemple: mysite-dev.
3. Cliquez sur "Enregistrer et déployer".

**Pratique :** découvrez l'interface et les fonctionnalités de Netlify.

## 6. Configurer le service DNS et les paramètres

**Pratique :** Distinguez le service de Domain Registrar et le service DNS. Révisez les [concepts DNS](https://en.wikipedia.org/wiki/Domain_Name_System).

**Pratique :** Apprenez [ce qu'est le fournisseur Cloudflare](https://blog.cloudflare.com/what-is-cloudflare/).

1. Obtenez un nom de domaine (https://www.ovh.com/fr/domaines/): par exemple, `example.com`.
2. Choisissez les adresses IP Cloudflare NS.
3. Choisissez un service DNS (https://www.cloudflare.com/).
4. Créez un CNAME `monsite mysite-dev.netlify.com`.

## 7. Configurez un domaine personnalisé

Dans l'interface Web frontale Netlify, configurez un domaine personnalisé:

1. Allez dans "mysite / settings / general".
2. Cliquez sur le bouton "Change site name" : par exemple "mysite".
3. Allez dans "Settings / Domain management / Domains".
4. Cliquez sur le bouton "Ajouter un domaine personnalisé": "mysite.example.com".

## 8. Sécurisez votre site avec HTTPS

**Pratique :** Revoir les concepts de sécurité et de certificats HTTPS.

**Pratique :** En savoir plus sur [Let's Encrypt](https://letsencrypt.org/about/). Let's Encrypt est une autorité de certification (CA) gratuite, automatisée et ouverte, exploitée pour le bénéfice du public. C'est un service fourni par [Internet Security Research Group (ISRG)](https://letsencrypt.org/isrg/).

Let's Encrypt donne aux gens les certificats numériques dont ils ont besoin pour activer HTTPS (SSL / TLS) pour les sites Web, gratuitement, de la manière la plus conviviale possible. Nous faisons cela parce que nous voulons créer un site Web plus sûr et plus respectueux de la vie privée.

Dans l'interface Web frontale de Netlify, sécurisez votre site avec HTTPS:

1. Allez dans Paramètres / Gestion de domaine / HTTPS.
2. Vérifiez que le DNS est correctement configuré avant d'activer HTTPS: cliquez sur le bouton "Vérifier la configuration DNS".
3. Fournissez un certificat pour votre domaine et activez HTTPS: cliquez sur le bouton "provisionner un certificat pour votre domaine et activer HTTPS".
4. Cliquez sur "Forcer HTTPS" après la génération du certificat.

## 9. Personnalisez votre site

**Pratique :** Passez en revue git avec https://try.github.io/ ou avec https://git-scm.com/book/en/v2/.

**Pratique :** [Apprenez le langage Markdown](https://www.markdowntutorial.com/): Markdown est essentiellement une syntaxe pour un format de texte simple, facile à lire, qui est conçu pour être converti en HTML ([source](https://www.oreilly.com/ideas/static-site-generators)). La plupart des moteurs de blogs ont commencé à offrir un support pour Markdown, y compris Wordpress.

**Pratique :** Installez localement un outils de développement web qui offrent un support Markdown prêt à l'emploi, comme [Sublime Text](http://www.sublimetext.com/), [Atom](https: // atom. io /), [Visual Studio Code](https://code.visualstudio.com/), ou [Brackets](http://brackets.io/).

Localement, personnalisez votre site et déployez-le:

1. Cloner localement le "repository" `https://github.com/myaccount/mysite-dev/`.
2. Ajoutez des pages de contenu écrites dans Markdown dans le répertoire `docs/`.
3. Configurez le fichier `mkdocs.yml` et ajoutez la partie récapitulative.
4. Validez et appuyez sur votre nouveau code avec `git`.

```bash
git clone https://github.com/myaccount/mysite-dev/
cd mysite-dev
vi docs /index.md
vi mkdocs.yml
git add *
git commit -m "personnalisation de site"
git push
```

Veuillez revenir à votre interface Web NetLify pour vérifier votre build et le déploiement du site Web.

Note: Vous pouvez trouver de belles photos de qualité sur https://unsplash.com/ (gratuit). Vous pouvez optimiser et transformer des images avec https://snappa.com/ (commercial).

## 10. Aller plus loin avec les générateurs de sites statiques.

**Pratique :** Revoir [théorie des motifs MVC](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller), [concepts CSS](https: // fr .wikipedia.org / wiki / Cascading_Style_Sheets), [langage HTML](https://en.wikipedia.org/wiki/HTML) et [concepts SEO](https://en.wikipedia.org/wiki/Search_engine_optimization).

Allez plus loin avec vos nouvelles compétences:

1. Créez un ID de suivi [Google Analytics](https://analytics.google.com/).
2. Créez un site dans votre compte [disqus](https://disqus.com/admin/).
3. Enregistrez le site sur [Google Search Console](https://www.google.com/webmasters/tools/home?hl=fr&pli=1) et lancez l'indexation du site.
4. Créez un `docs/images/` pour stocker des images.
5. Intégrez un formulaire Mailchimp ou un widget Twitter, ou ajoutez un bloc de bannière AdSense.
6. [Modifier le thème MkDocs](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Themes) et/ou exploiter leur CSS.
7. Validez votre site avec [Woorank](https://www.woorank.com/).
