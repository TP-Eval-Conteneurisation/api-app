# Projet de Documentation

## Description
Ce projet est conçu pour [description du projet]. Il permet de [fonctionnalités principales].

## Installation

## GitHub Actions Workflow

### Emplacement du workflow
Le workflow CI/CD se trouve dans le fichier `.github/workflows/docker-build.yml`.

### Fonctionnement du workflow
Ce workflow automatise les processus suivants :
- Déclenchement lors des push sur la branche `main` et des pull requests vers `main`
- Installation des dépendances Node.js
- Exécution des tests
- Construction de l'image Docker
- Publication de l'image sur GitHub Container Registry (seulement lors des push sur `main`)

### Interprétation des résultats
1. Accédez à l'onglet "Actions" sur votre dépôt GitHub
2. Sélectionnez le workflow "Docker Build and Push (CI-CD)"
3. Vérifiez le statut de chaque run (✅ vert pour succès, ❌ rouge pour échec)
4. Cliquez sur un run spécifique pour voir les détails de chaque étape
5. En cas de publication réussie, l'image sera disponible à `ghcr.io/[owner]/[repo]/api-app:latest`
