# 🥃 Saloon – Gestion de stock et point de vente

[![Démo en ligne](https://img.shields.io/badge/Démo-mekeirish.github.io%2FSaloon-brightgreen)](https://mekeirish.github.io/Saloon/)
[![Licence](https://img.shields.io/badge/Licence-MIT-blue)](./LICENSE)
[![PWA](https://img.shields.io/badge/PWA-ready-success)](https://mekeirish.github.io/Saloon/)

> **Saloon** est une application web progressive (PWA) de gestion de stock et de ventes, pensée pour les petits commerces (salons, bars, boutiques). Elle permet de suivre l’inventaire, d’enregistrer les opérations, de visualiser les statistiques en temps réel et de personnaliser l’interface selon vos préférences.

---

## 📋 Table des matières

- [Fonctionnalités](#-fonctionnalités)
- [Modes d’affichage](#-modes-daffichage)
- [Architecture technique](#-architecture-technique)
- [Installation locale](#-installation-locale)
- [Déploiement](#-déploiement)
- [Structure du projet](#-structure-du-projet)
- [Contribuer](#-contribuer)
- [Licence](#-licence)

---

## ✨ Fonctionnalités

- **État des stocks** : inventaire et quantités disponibles en temps réel, avec seuil d’alerte personnalisable.
- **Statistiques de ventes** : chiffre d’affaires du jour, évolution mensuelle et recette du jour.
- **Objectif journalier** : barre de progression vers un objectif de CA défini.
- **Enregistrement des opérations** : ajout, modification et suivi des ventes avec historique global.
- **Historique complet** : consultation de toutes les opérations enregistrées, avec possibilité d’export et d’archivage.
- **Gestion des produits** : édition des carreaux (produits) avec prix d’achat, marge et stock.
- **Stockage distant des images** : intégration d’une clé API ImgBB pour héberger les visuels des produits.
- **Personnalisation avancée** :
  - Ambiance « Saloon » (halo doré et particules).
  - Mode « Easy Vision » avec miniatures de ticket.
  - Grands caractères pour améliorer la lisibilité.
  - Effets sonores et retour haptique (vibration) sur mobile.
- **PWA installable** : fonctionnement hors ligne partiel, icône et écrans de démarrage personnalisés, thème sombre `#010104`.

---

## 🎛 Modes d’affichage

L’application propose plusieurs modes adaptés à différents usages.  
La page d’accueil invite à **« Choisissez votre mode »** pour ajuster la grille de produits (colonnes et lignes) et l’affichage selon vos besoins.

---

## 🛠 Architecture technique

| Élément | Détail |
|---------|--------|
| **Type** | Application web monopage (SPA) / PWA |
| **Fichier principal** | `index.html` (interface complète, styles et logique intégrés) |
| **Manifeste PWA** | `manifest.json` – nom « Saloon », mode `standalone`, thème sombre `#010104` |
| **Icônes** | `icon-192.png` (192×192), `icon.png` (512×512, maskable) |
| **Écrans de démarrage** | Plusieurs résolutions (`splash-*.png`) pour un rendu natif sur mobile |
| **Déploiement** | GitHub Pages (branche `main`) |

---

## 💻 Installation locale

Aucune dépendance ni build n’est nécessaire. Il suffit de cloner le dépôt et d’ouvrir `index.html` dans un navigateur.

```bash
git clone https://github.com/mekeirish/Saloon.git
cd Saloon
# Ouvrir index.html dans votre navigateur
# ou lancer un serveur local (recommandé pour tester la PWA) :
python3 -m http.server 8080
# puis ouvrir http://localhost:8080
```

---

## 🌐 Déploiement

Le site est automatiquement publié sur **GitHub Pages** à chaque mise à jour de la branche `main` :

👉 **[https://mekeirish.github.io/Saloon/](https://mekeirish.github.io/Saloon/)**

---

## 📁 Structure du projet

```text
Saloon/
├── index.html                 # Application complète (UI + logique)
├── manifest.json              # Manifeste PWA
├── icon.png                   # Icône 512×512
├── icon-192.png               # Icône 192×192
├── splash-*.png               # Écrans de démarrage mobiles
└── README.md
```

---

## 🤝 Contribuer

Les contributions sont les bienvenues !  
Pour proposer une amélioration ou signaler un bug :

1. Ouvrez une **issue** en décrivant clairement le problème ou la suggestion.
2. Forkez le dépôt, créez une branche (`feature/ma-fonctionnalite`) et soumettez une **pull request**.
3. Assurez-vous que les modifications restent compatibles avec le déploiement GitHub Pages et la PWA.

---

## 📄 Licence

Ce projet est distribué sous licence **MIT**.  
Voir le fichier [`LICENSE`](./LICENSE) pour plus de détails.

---

**Saloon** – Une solution simple et centralisée pour digitaliser la gestion des stocks et des ventes de votre commerce.