# 🏝️ Verdhame — Un univers de test pour Maître de Jeu IA

## 1. Qu'est-ce que Verdhame ?

Verdhame est un projet expérimental visant à évaluer les capacités d'une intelligence artificielle à agir comme **Maître de Jeu (MJ)** dans un univers de jeu de rôle persistant.

L'univers se déroule sur l'île fictive de **Verdhame**, un territoire partagé entre trois factions rivales :

* 🌲 **Les Hévalords** — gardiens des forêts du nord
* ⚒️ **La Cité de Fer** — puissance marchande et industrielle du centre
* 🌫️ **Le Clergé des Brumes** — théocratie mystérieuse des marais du sud

L'ensemble du monde est menacé par un phénomène surnaturel appelé **la Tempête des Brumes**, dont l'intensité évolue au cours de la partie.

Le joueur doit explorer l'île, interagir avec les factions et retrouver les **Reliques de l'Équilibre** afin d'empêcher la catastrophe.

---

## 2. Objectifs du projet

L'objectif principal n'est pas de créer un jeu vidéo, mais de fournir un **cadre d'expérimentation pour les LLMs**.

Verdhame permet notamment d'évaluer :

### 🧠 Mémoire

L'IA est-elle capable de conserver l'état du monde sur plusieurs dizaines de tours ?

* progression du joueur
* alliances
* quêtes
* événements passés
* conséquences des choix

### 📋 Planification

L'IA est-elle capable de :

* gérer une quête principale
* maintenir des objectifs à long terme
* préparer des événements futurs
* faire évoluer les factions

### 🎲 Respect des règles

Le MJ doit suivre un ensemble de règles définies :

* structure des tours
* système de combat
* gestion des quêtes
* évolution du personnage
* conditions de victoire et de défaite

### 🌍 Cohérence narrative

Les actions du joueur doivent produire des conséquences crédibles et persistantes dans le monde.

---

## 3. Contenu du dépôt

```text
.
├── Ressources
│   └── Carte de verdhame.png
│
├── context
│   ├── univers.md
│   ├── bestiaire.md
│   └── competences.md
│
├── memory
│   ├── joueur.md
│   └── chronique_partie1.md
│
├── skills
│   ├── tour.md
│   ├── combat.md
│   └── quete.md
│
└── CLAUDE.md
```

### 📖 context/

Contient les informations statiques du monde :

* lore
* factions
* créatures
* compétences
* contexte narratif

### 💾 memory/

Contient les informations évolutives de la partie :

* état du joueur
* progression
* historique des événements

### ⚙️ skills/

Décrit les règles de fonctionnement du MJ :

* déroulement d'un tour
* résolution des actions
* système de combat
* gestion des quêtes

### 🗺️ Ressources/

Contient les supports visuels utilisés par le MJ.

---

## 4. Principe de fonctionnement

Le système repose sur une boucle de jeu stricte.

### Étape 1 — Narration

Le MJ décrit :

* le lieu
* les personnages présents
* l'ambiance
* les événements en cours

### Étape 2 — Action du joueur

Le joueur agit librement.

Aucune liste d'actions n'est imposée.

### Étape 3 — Résolution

Le MJ :

* détermine la caractéristique utilisée
* effectue les jets nécessaires
* applique les conséquences
* met à jour les relations et l'état du monde

### Étape 4 — Mise à jour de la mémoire

Les fichiers de mémoire sont mis à jour :

* PV
* XP
* inventaire
* alliances
* progression des quêtes
* état de la Tempête

### Étape 5 — Vérification des conditions de fin

Le MJ vérifie :

* victoire
* défaite
* progression de quête

Puis un nouveau tour commence.

---

## 5. Axes d'amélioration

Le projet est volontairement simple afin de servir de laboratoire d'expérimentation.

Plusieurs évolutions sont envisagées :

### 🧑 PNJ persistants

Ajout d'une mémoire dédiée aux personnages importants :

* relations
* objectifs
* évolution dans le temps

### 🌍 État global du monde

Séparation de l'état du joueur et de l'état du monde :

* puissance des factions
* niveau de la Tempête
* événements mondiaux

### 📜 Gestion avancée des quêtes

* quêtes secondaires
* événements dynamiques
* embranchements narratifs

### 🧠 Mémoire long terme

Évaluation de la capacité des modèles à réutiliser des informations découvertes plusieurs dizaines de tours auparavant.

### 🤖 Compatibilité multi-modèles

Tester différents modèles de langage sur une même campagne afin de comparer :

* cohérence
* mémoire
* créativité
* respect des règles

---

## Pourquoi ce projet ?

Verdhame est avant tout une expérience.

L'objectif est de fournir un environnement suffisamment riche pour mettre à l'épreuve les capacités de raisonnement, de mémoire et de narration des IA modernes, tout en restant suffisamment compact pour être compris et modifié facilement.

En résumé : **un bac à sable de jeu de rôle conçu pour tester les capacités d'un Maître de Jeu IA.**
