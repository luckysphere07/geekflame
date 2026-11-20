# GeekFlame 🔥

Site tech bilingue **français / anglais** consacré à la domotique, au homelab, à l'IA et aux tutoriels informatiques.

- Domaine acheté : `geek-flame.com` (Cloudflare).
- Générateur : Hugo 0.146+.
- Langues : `/fr/` et `/en/`.
- État : **préparation uniquement**, pas de publication publique validée.
- Le premier guide Zigbee2MQTT est un **brouillon** (`draft: true`).
- Le paramètre `launchReady = false` désactive l'indexation ; ne pas le modifier sans validation.

## Utilisation locale

```bash
hugo server -D
hugo --minify
```

Ouvrir `http://localhost:1313/fr/` et `http://localhost:1313/en/`. Le dossier produit par la compilation est `public/`.

## Publication

Voir [DEPLOIEMENT.md](DEPLOIEMENT.md). Le site cible **Cloudflare Workers Static Assets**. Vérifier le rendu et les mentions légales avant de connecter le domaine principal.

## Ajouter un article

Créer les versions en `content/fr/articles/` et `content/en/articles/`, avec un même `translationKey`. Toujours valider les étapes et les captures avant de changer `draft: true`.

## À finaliser

Mentions légales, confidentialité, adresse de contact, traduction et validation technique des guides. Aucune publicité ni tracking activés dans ce kit.
