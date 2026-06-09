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
## 2. Objectifs

Ce dépôt a pour objectif de fournir un environnement de test permettant d'évaluer le comportement d'un modèle de langage lorsqu'il est utilisé comme Maître de Jeu (MJ) dans un jeu de rôle textuel.

Le projet vise notamment à observer :

* la capacité du modèle à maintenir un état cohérent du monde au fil des interactions ;
* la gestion d'informations persistantes (personnage, factions, progression, événements passés) ;
* le respect de règles définies dans des documents séparés ;
* la cohérence des conséquences produites par les actions du joueur ;
* la gestion d'objectifs à court et long terme au sein d'une campagne.

L'univers de Verdhame constitue un cadre d'expérimentation volontairement limité afin de faciliter l'analyse des comportements du modèle.

---

## 3. Structure du dépôt

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

### context/

Contient les informations de référence nécessaires au fonctionnement du monde de jeu :

* description de l'univers ;
* factions et contexte narratif ;
* bestiaire ;
* compétences disponibles.

Ces fichiers sont considérés comme des données statiques.

### memory/

Contient les informations évolutives produites au cours d'une partie :

* état du personnage ;
* progression ;
* événements importants ;
* historique de campagne.

Ces fichiers représentent la mémoire persistante du système.

### skills/

Décrit les règles opérationnelles que le Maître de Jeu doit appliquer :

* déroulement d'un tour ;
* résolution des combats ;
* progression de quête ;
* conditions de victoire et de défaite.

### Ressources/

Contient les éléments visuels utilisés pour enrichir l'univers ou faciliter la représentation du monde.

---

## 4. Principe de fonctionnement

Le système repose sur une séparation explicite entre les données du monde, les règles du jeu et la mémoire de la partie.

Chaque interaction suit le cycle défini dans `skills/tour.md` :

1. Description de la situation courante.
2. Réception de l'action du joueur.
3. Résolution de l'action selon les règles applicables.
4. Mise à jour de l'état persistant.
5. Vérification des conditions de progression ou de fin de partie.

Le rôle du modèle est d'agir comme un moteur narratif tout en respectant les contraintes définies dans le dépôt.

Les décisions du joueur peuvent modifier :

* les relations entre factions ;
* l'évolution de la Tempête des Brumes ;
* la progression de la quête principale ;
* l'état du personnage ;
* certains événements futurs.

L'ensemble de ces modifications doit être répercuté dans les fichiers de mémoire afin de garantir la continuité de la campagne.

---

## 5. Axes d'amélioration

Le projet constitue une base expérimentale susceptible d'être étendue selon plusieurs directions.

### Gestion avancée de l'état du monde

* séparation complète entre état du joueur et état global ;
* suivi de l'évolution des factions ;
* événements dynamiques influencés par les actions passées.

### Gestion des personnages non-joueurs

* mémoire dédiée aux PNJ ;
* suivi des relations ;
* objectifs individuels ;
* évolution autonome au fil de la campagne.

### Extension du système de quêtes

* quêtes secondaires ;
* événements conditionnels ;
* embranchements narratifs multiples.

### Évaluation des capacités des modèles

Le dépôt peut être utilisé pour comparer différents modèles de langage selon plusieurs critères :

* cohérence narrative ;
* respect des règles ;
* qualité de la mémoire à long terme ;
* gestion de la progression ;
* stabilité des décisions.

### Outillage et automatisation

* validation automatique des mises à jour de mémoire ;
* suivi des états de partie ;
* métriques de cohérence ;
* scénarios de test reproductibles.
