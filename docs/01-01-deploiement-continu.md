# 1. Le déploiement continu

## 1. Qu'est-ce le déploiement continu ?

!!! info "Définition"
    Le déploiement continu peut être considéré comme une extension de [l'intégration continue](https://www.agilealliance.org/glossary/continuous-integration/) (CI), visant à minimiser [délai d'exécution](https://www.agilealliance.org/glossary/lead-time/), soit le temps écoulé entre le développement d'une nouvelle ligne de code et l'utilisation de ce nouveau code par les utilisateurs en production. [^continuous-deployment]

[^continuous-deployment]: [Défintion de la notion de déploiement continu par l'Agile Alliance](https://www.agilealliance.org/glossary/continuous-deployment/)

!!! cite "Livraison continue (Continuous Delivery) "
    La **livraison continue** est une suite de pratiques conçues pour garantir que le code peut être déployé rapidement et en toute sécurité vers la production en livrant chaque changement dans un environnement proche de la production et en garantissant que les applications et services métier fonctionnent comme prévu grâce à des tests automatisés rigoureux. Comme chaque modification est fournie à un environnement intermédiaire en utilisant une automatisation complète, vous pouvez avoir l'assurance que l'application peut être déployée en production en appuyant sur un bouton lorsque tout est prêt.
    Le **déploiement continu** est la prochaine étape de la livraison continue: chaque modification qui passe les tests automatisés est automatiquement déployée en production. Le déploiement continu devrait être l'objectif de la plupart des entreprises qui ne sont pas limitées par des exigences réglementaires ou autres. [^continuous-delivery]
    ![](https://puppet.com/sites/default/files/2016-09/puppet_continuous_diagram.gif)


[^continuous-delivery]: [Puppet blog Continuous Delivery Vs. Continuous Deployment: What's the Diff?](https://puppet.com/blog/continuous-delivery-vs-continuous-deployment-what-s-diff).
