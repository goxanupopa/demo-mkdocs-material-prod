# 1. Le déploiement continu

## Qu'est-ce Devops ?

Le mouvement devops est né d'une part de la volonté de globaliser les méthodes agiles à l'ensemble du système d'information et d'autre part de l'application des principes de l'agilité à la production. Il est cependant possible d'être agile dans une équipe uniquement de développement, comme il est possible de mettre en place certains principes devops dans un environnement de développement en cascade.

* DevOps s'appuie sur la méthode Scrum en intégrant l'ensemble des principes agiles : Daily Scrum Meeting, Product backlog, Sprints, Product Owner, Scrum Master, Rétrospectives des Sprints.
* DevOps met en œuvre les principes du Lean Management de façon à simplifier les travaux des développeurs et des administrateurs pour ensuite les automatiser sur des outils transversaux.
* DevOps met en place les processus ITSM en les simplifiant et les adaptant aux contextes de l'entreprise (Gestion des changements, Gestion des actifs et des configurations, Gestion des mises en production et des déploiements, Gestion des incidents, Gestion des problèmes, Gestion de la connaissance...)

!!! info "Définition Devops"
    Devops est la concaténation des trois premières lettres du mot anglais development (développement) et de l'abréviation usuelle ops du mot anglais operations (exploitation), deux fonctions de la gestion des systèmes informatiques qui ont souvent des objectifs contradictoires. Le mot a été inventé par Patrick Debois1 durant l'organisation des premiers devopsdays à Gand en Belgique, en octobre 2009. Le DevOps est un mouvement visant à l'alignement de l'ensemble des équipes du système d'information sur un objectif commun, à commencer par les équipes de dev ou dev engineers chargés de faire évoluer le système d'information et les ops ou ops engineers responsables des infrastructures (exploitants, administrateurs système, réseau, bases de données,...). Ce qui peut être résumé par : travailler ensemble pour produire de la valeur pour l'entreprise. [^devops-wikipedia]

[^devops-wikipedia]: [Définition Devops de Wikipedia FR](https://fr.wikipedia.org/wiki/Devops)

## Qu'est-ce le déploiement continu ?

Déploiement continu, livraison continue (CD) et intégration continue sont un ensemble de pratiques liées à des outils et/ou des services d'usines logicielles relevant du mouvement plus large appelé "Devops".

!!! info "Définition du déploiement continu"
    Le déploiement continu peut être considéré comme une extension de [l'intégration continue](https://www.agilealliance.org/glossary/continuous-integration/) (CI), visant à minimiser [délai d'exécution](https://www.agilealliance.org/glossary/lead-time/), soit le temps écoulé entre le développement d'une nouvelle ligne de code et l'utilisation de ce nouveau code par les utilisateurs en production. [^continuous-deployment]

[^continuous-deployment]: [Défintion de la notion de déploiement continu par l'Agile Alliance](https://www.agilealliance.org/glossary/continuous-deployment/)

!!! cite "Livraison continue (Continuous Delivery) "
    La **livraison continue** est une suite de pratiques conçues pour garantir que le code peut être déployé rapidement et en toute sécurité vers la production en livrant chaque changement dans un environnement proche de la production et en garantissant que les applications et services métier fonctionnent comme prévu grâce à des tests automatisés rigoureux. Comme chaque modification est fournie à un environnement intermédiaire en utilisant une automatisation complète, vous pouvez avoir l'assurance que l'application peut être déployée en production en appuyant sur un bouton lorsque tout est prêt.
    Le **déploiement continu** est la prochaine étape de la livraison continue : chaque modification qui passe les tests automatisés est automatiquement déployée en production. Le déploiement continu devrait être l'objectif de la plupart des entreprises qui ne sont pas limitées par des exigences réglementaires ou autres. [^continuous-delivery]
    ![](https://puppet.com/sites/default/files/2016-09/puppet_continuous_diagram.gif)

[^continuous-delivery]: [Puppet blog Continuous Delivery Vs. Continuous Deployment: What's the Diff?](https://puppet.com/blog/continuous-delivery-vs-continuous-deployment-what-s-diff).
