# Pipeline CI/CD - Automatisation du déploiement

## Description du projet

Ce projet vise à automatiser le déploiement d'une application Java Spring Boot :  
**Mini Projet - Système de Gestion de Bibliothèque**  
Développée pour gérer les opérations d’une bibliothèque (gestion des livres, des membres, des prêts, etc.).

L’objectif principal est de mettre en place une pipeline CI/CD complète permettant de garantir des déploiements rapides, fiables et reproductibles dans un environnement cloud Kubernetes.

---

## Technologies utilisées

- **Java, Spring Boot** : Application métier backend.
- **Git** : Gestion du code source.
- **Jenkins** : Orchestration de la pipeline CI/CD, installé sur un serveur dédié.
- **Docker** : Conteneurisation de l’application, sur un serveur Docker dédié.
- **Ansible** : Automatisation de la configuration et du déploiement.
- **Azure Cloud** : Infrastructure cloud utilisée.
- **Azure Kubernetes Service (AKS)** : Orchestration des conteneurs Docker.

---

## Fonctionnalités de la pipeline CI/CD

- Intégration continue avec compilation, tests unitaires et d’intégration automatiques.
- Construction et publication d’images Docker dans Azure Container Registry (ACR).
- Déploiement automatisé et mise à jour de l’application dans AKS.
- Gestion de la configuration d’infrastructure via Ansible.
- Jenkins installé sur un serveur dédié pour gérer les pipelines.
- Docker exécuté sur un serveur dédié pour construire et héberger les conteneurs.
- Monitoring et notifications post-déploiement.

---

## Dépôt du projet

Le code source de l’application Java Spring Boot est disponible ici :  
[https://github.com/1-thegreenprogrammer/library-management-system](https://github.com/1-thegreenprogrammer/library-management-system)

---

## Structure du projet

- `/src` : Code source Java Spring Boot.
- `Jenkinsfile` : Pipeline Jenkins décrivant les étapes CI/CD.
- `ansible/` : Playbooks Ansible pour l’automatisation des déploiements.
- `k8s/` : Manifests Kubernetes pour le déploiement dans AKS.
- `Dockerfile` : Construction de l’image Docker de l’application.

---

## Instructions pour lancer la pipeline

1. **Commit & Push** du code sur le dépôt Git.
2. Jenkins (sur serveur dédié) détecte la modification et déclenche la pipeline.
3. Compilation et tests automatiques s’exécutent.
4. Image Docker est construite sur le serveur Docker dédié puis poussée vers Azure Container Registry.
5. Ansible configure l’environnement AKS.
6. Déploiement automatique dans le cluster Kubernetes AKS.
7. Notifications envoyées sur le succès ou l’échec du déploiement.

---

## Résultats attendus

- Déploiements plus rapides et fiables.
- Réduction des erreurs manuelles.
- Environnement cohérent et reproductible.
- Amélioration de la productivité des équipes de développement et opérationnelles.

---

## Contact

Pour toute question ou collaboration :  
[1-thegreenprogrammer@gmail.com]

---

*Ce projet a été réalisé entre Janvier 2025 et Avril 2025 dans le cadre d’une automatisation CI/CD sur Azure.*

