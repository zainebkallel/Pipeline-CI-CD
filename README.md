# Pipeline CI/CD avec Jenkins, Ansible et Kubernetes

## Description

Ce projet met en œuvre un pipeline CI/CD permettant d'automatiser le déploiement d'une application Spring Boot sur un cluster Kubernetes.

Le pipeline assure les étapes suivantes :

- Récupération du code source depuis GitHub
- Compilation de l'application avec Maven
- Construction de l'image Docker
- Publication de l'image sur Docker Hub
- Déploiement automatique sur Kubernetes via Ansible
- Vérification du déploiement et de l'exposition des métriques Prometheus

## Technologies utilisées

- Jenkins
- Maven
- Docker
- Docker Hub
- Ansible
- Kubernetes
- Spring Boot
- Prometheus

## Structure du projet

```
.
├── Jenkinsfile
├── playbookCICD.yml
├── deployment.yaml
├── service.yaml
├── hosts
└── README.md
```

## Fonctionnement

1. Jenkins récupère le code source depuis GitHub.
2. L'application est compilée avec Maven.
3. Ansible construit et publie l'image Docker.
4. Les ressources Kubernetes (Deployment et Service) sont déployées.
5. Jenkins vérifie que l'application est accessible et que les métriques Prometheus sont disponibles.

## Auteur

**Zaineb Kallel**
