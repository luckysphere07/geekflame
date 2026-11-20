# Déploiement GeekFlame — préparation

Dépôt : https://github.com/luckysphere07/geekflame

## Hébergement prévu

Cloudflare Workers + Static Assets (nouveau projet, distinct des Workers existants).

1. Installer Hugo **0.146 ou plus récent** en local, puis tester `hugo --minify`.
2. Vérifier `public/fr/index.html`, `public/en/index.html`, `robots.txt` et les liens de langue.
3. Dans Cloudflare Workers & Pages, ouvrir la rubrique de création d'application, connecter le dépôt GitHub `luckysphere07/geekflame`.
4. Configurer le build Hugo pour produire le dossier `public/`, puis le servir comme *static assets*. Utiliser la version et les paramètres proposés par Cloudflare.
5. Vérifier sur une adresse **de prévisualisation uniquement** avant toute association à `geek-flame.com`.

Le compte Cloudflare n'avait pas encore de sous-domaine `workers.dev` initialisé lors du contrôle du 20/11/2026. L'activation initiale peut être nécessaire dans l'interface.

**Ne pas modifier les enregistrements DNS, les routes ni l'indexation sans validation.** `launchReady = false` reste actif. Les pages légales sont des brouillons.

Documentation : https://developers.cloudflare.com/workers/static-assets/ et https://developers.cloudflare.com/workers/ci-cd/builds/
