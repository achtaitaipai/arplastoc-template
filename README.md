# Template Arplastoc

Un dépôt pour permettre aux enseignants de démarrer un site statique sur le modèle de [Arplastoc](https://arplastoc.com).

## Mise en ligne

Pour la mise en ligne vous aurez au préalable besoin de posséder un compte [Github](https://github.com/)

[![Mettre en ligne sur Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/arplastoc/site)

## Mise en place de l'éditeur de contenu

**Arplastoc** utilise l'éditeur de contenu `keystatic` et son service `keystatic cloud`, pour pouvoir y accéder vous devrez créer un compte sur [keystatic Cloud](https://keystatic.cloud).

1. Créez ensuite une `team` puis un `project` avec les noms que vous désirez. 
2. Reliez votre projet au dépôt github (probablement: `arplastoc-template`) que vous venez de créer.
3. Renseignez l'url de votre site (vous pourrez modifier celui-ci plus tard).
4. Retournez sur netlify, dans `Site configuration` sélectionnez `Environment variables`, puis `Add a variable`. Dans le champs `key` entrez `PUBLIC_KEYSTATIC_CLOUD_PROJECT`, puis dans valeur le nom de votre `team` suivi d'un slash `/` suivi du nom de votre `project` keystatic. Par exemple: `mateam/monprojet`
5. Sur netlify retournez dans `site overview`, `Production deploys` et cliquez sur `Trigger deploy`, puis `Deploy site`.

Lorsque le déploiement aura pris fin vous devriez pouvoir accéder à l'éditeur de contenu, en vous rendant à l'url de votre site et en ajoutant `/keystatic`. Par exemple: `https://monsite.netlify.app/keystatic` 