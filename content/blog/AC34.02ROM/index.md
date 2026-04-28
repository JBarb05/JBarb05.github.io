---
title: "AC34.02ROM Administrer et déployer des fonctions réseaux virtualisées et programmer le réseau"
date: 2026-04-28
summary: "Réflexion personnelle sur la virtualisation des fonctions réseau, la programmabilité et l’automatisation dans un parcours de professionnalisation en BUT Réseaux & Télécommunications."
tags:
    - virtualisation
    - esxi
    - docker
    - ansible
    - automatisation
    - réseaux
authors:
    - me
featured: false

---

# Administrer et déployer des fonctions réseaux virtualisées et programmer le réseau

## Contexte
Cet apprentissage a été réalisé en cours dans le cadre de la compétence AC34.02ROM.  
Le sujet portait sur l’administration de fonctions réseau virtualisées, avec une mise en pratique via **VMware ESXi** pour la virtualisation de machines, **Docker** pour le déploiement de services conteneurisés et **Ansible** pour l’automatisation de la configuration et du déploiement.

## Réalisation
- Installation et prise en main d’un environnement virtualisé sous ESXi.  
- Création et configuration de machines virtuelles pour simuler une infrastructure réseau.  
- Déploiement de services réseau dans des conteneurs Docker (tests de lancement, réseau entre conteneurs, exposition de ports).  
- Mise en place de playbooks **Ansible** pour automatiser certaines tâches de configuration et de déploiement.  
- Vérification du fonctionnement global et validation de la connectivité entre les différents éléments.

## Preuves illustratives éventuelles
- Captures d’écran de l’hyperviseur ESXi (VM créées, ressources allouées).  
- Fichiers de configuration Docker / commandes utilisées (`docker run`, `docker ps`, `docker network ls`).  
- Playbooks Ansible et inventaires utilisés pour l’automatisation.  
- Schéma simple de l’architecture mise en place.  
- Résultats de tests réseau (ping, accès aux services).

## Analyse réflexive

### Réussites
- Bonne compréhension du lien entre virtualisation (ESXi), conteneurisation (Docker) et automatisation (Ansible).  
- Déploiement fonctionnel de services réseau dans un environnement virtualisé.  
- Amélioration de la méthode de test, de validation et d’automatisation.

### Difficultés
- Différences de fonctionnement entre machine virtuelle et conteneur au début.  
- Paramétrage réseau (interfaces, ports, réseaux Docker) parfois complexe.  
- Prise en main des playbooks Ansible et gestion des erreurs de configuration lors des premiers déploiements.

### Apprentissage
- Savoir choisir entre VM, conteneur et automatisation selon le besoin.  
- Mieux structurer un déploiement réseau virtualisé et automatisé.  
- Renforcer les compétences d’administration système/réseau et de diagnostic.

### Projection pour la suite
- Approfondir l’automatisation des déploiements avec **Ansible** (roles, templates, variables).  
- Tester des architectures plus complètes (plusieurs services interconnectés).  
- Se former à des outils complémentaires d’orchestration et de supervision.

## Note
**3/5**

## Bilan
Cette activité m’a permis de consolider des compétences concrètes en virtualisation réseau, en conteneurisation et en automatisation des déploiements. L’usage combiné de ESXi, Docker et Ansible constitue une base solide pour des projets d’infrastructure modernes.