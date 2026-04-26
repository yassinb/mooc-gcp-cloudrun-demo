# MOOC GCP Cloud Run Demo

Petit site web statique utilisé pour une démonstration CI/CD avec Google Cloud.

## Contenu

- `site/index.html` : page web
- `site/style.css` : style du site
- `Dockerfile` : image Nginx servant le site statique
- `cloudbuild.yaml` : pipeline Cloud Build

## Pipeline

Le fichier `cloudbuild.yaml` réalise les étapes suivantes :

1. Build de l'image Docker
2. Push dans Artifact Registry
3. Déploiement sur Cloud Run

## Cible

Service Cloud Run : `mooc-web`

Région : `europe-west1`
