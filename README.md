# 🌐 Projet GIT – Mini-site de Présentation d’Entreprise

## 🎯 Objectif
Ce projet a pour but de mettre en œuvre une gestion de version professionnelle avec Git, autour d’un mini-site statique (HTML/CSS/JS) développé individuellement.

---

## 🧠 Stratégie de branche utilisée

La stratégie de branches Git adoptée suit un flux de développement structuré et progressif :

- **`main`** : branche finale stable (code propre et validé, prêt à être publié)
- **`dev`** : branche d’intégration globale (contient toutes les fonctionnalités testées)
- **`test/frontend`** : branche pour les tests d’intégration (HTML, CSS, JS)
- **`feature/html-structure`** : branche dédiée à la structure HTML du site
- **`feature/css-theme`** : branche pour la charte graphique CSS (polices, couleurs, responsive)
- **`feature/js-interactions`** : branche pour les fonctionnalités dynamiques (JS)

### 🔁 Flux de travail appliqué :
```text
feature/* → test/frontend → dev → main
Étapes suivies

    Initialisation du dépôt Git

        git init

        git checkout -b main

        git checkout -b dev

    Développement des fonctionnalités par branches feature/*

        feature/html-structure : structure HTML des pages (index.html, services.html, contact.html)

        feature/css-theme : création de style.css, mise en page, responsive

        feature/js-interactions : interactions JS (carrousel, menu burger, scroll)

    Tests d’intégration dans test/frontend

        Fusion des branches feature/*

        Tests visuels et fonctionnels dans le navigateur

    Fusion dans la branche dev

        Après validation des tests, intégration dans dev

    Fusion finale dans main

        Code final propre, testé et prêt à être publié
        Commandes Git utilisées
Commande	Description
git init	Initialiser le dépôt Git
git branch	Lister les branches
git checkout -b <nom>	Créer et basculer sur une nouvelle branche
git add .	Ajouter tous les fichiers modifiés/stagés
git commit -m "Message"	Créer un commit avec un message clair
git merge <branche>	Fusionner une branche dans la branche courante
git status	Vérifier l’état du dépôt (fichiers modifiés, etc.)
git log	Afficher l’historique des commits
git push	Envoyer les commits sur GitHub
git pull	Récupérer les dernières modifications