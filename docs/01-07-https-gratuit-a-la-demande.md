# 7. HTTPS gratuit à la demandes

## 1. Sécurisez votre site avec HTTPS

**Pratique :** Revoir les concepts de sécurité et de certificats HTTPS.

**Pratique :** En savoir plus sur [Let's Encrypt](https://letsencrypt.org/about/). Let's Encrypt est une autorité de certification (CA) gratuite, automatisée et ouverte, exploitée pour le bénéfice du public. C'est un service fourni par [Internet Security Research Group (ISRG)](https://letsencrypt.org/isrg/).

>Let's Encrypt offre à quiconque les certificats numériques dont il a besoin pour activer HTTPS (SSL/TLS) pour des sites Web, gratuitement, de la manière la plus conviviale possible. Let's Encrypt veut donner la possibilité de créer des sites Web plus sûrs et plus respectueux de la vie privée.

Dans l'interface Web frontale de Netlify, sécurisez votre site avec HTTPS :

1. Allez dans "Settings / Domain management / HTTPS".
2. Vérifiez que le DNS est correctement configuré avant d'activer HTTPS: cliquez sur le bouton "Verify DNS Configuration".
3. Fournissez un certificat pour votre domaine et activez HTTPS: cliquez sur le bouton "Provision a certificate for your domain and enable HTTPS".
4. Cliquez sur "Force HTTPS" après la génération du certificat pour forcer HTTPS.
