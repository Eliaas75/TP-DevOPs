# TP-DevOPs

Mini projet Node.js réalisé dans le cadre d’un TP DevOps, avec mise en place d’une pipeline CI/CD complète via GitHub Actions.

## Objectif

Ce projet a pour but de démontrer la mise en place d’une chaîne DevOps simple autour d’une application Node.js :

- exécution automatisée des tests
- build Docker
- scan de sécurité
- déploiement simulé

## Fonctionnalités

L’application expose 3 routes HTTP :

- `/` : retourne un statut `ok` et le résultat d’une addition
- `/health` : retourne un statut de santé de l’application
- `/metrics` : retourne des métriques au format Prometheus

## Structure du projet

```text
.
├── .github/
│   └── workflows/
│       └── ci.yml
├── src/
│   ├── index.js
│   └── math.js
├── test/
│   └── math.test.js
├── .gitignore
├── Dockerfile
├── package-lock.json
├── package.json
└── README.md
