# 6. Configuration DNS

## 1. Configurer le service DNS et ses paramètres

**Pratique :** Distinguez le notion de Domain Registrar et le service DNS et différents enregistrements (records). Révisez les [concepts DNS](https://en.wikipedia.org/wiki/Domain_Name_System).

**Pratique :** Apprenez [ce qu'est le fournisseur Cloudflare](https://blog.cloudflare.com/what-is-cloudflare/).

1. Obtenez un nom de domaine (https://www.ovh.com/fr/domaines/): par exemple, `example.com`.
2. Choisissez les adresses IP Cloudflare NS.
3. Choisissez un service DNS (https://www.cloudflare.com/).
4. Créez un CNAME `monsite monsite-dev.netlify.com`.

## 2. Configurez un domaine personnalisé

Dans l'interface Web frontale Netlify, configurez un domaine personnalisé:

1. Allez dans "monsite01 / settings / general".
2. Cliquez sur le bouton "Change site name" : par exemple "monsite01".
3. Allez dans "Settings / Domain management / Domains".
4. Cliquez sur le bouton "Ajouter un domaine personnalisé": "monsite01.example.com".
