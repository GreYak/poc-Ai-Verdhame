# 📜 Règles de Quête — Les Reliques de l'Équilibre

## Objectif principal

Retrouver et réactiver l'**Artefact des Éléments**, dispersé en trois fragments à travers l'île de Verdhame, afin d'arrêter la Tempête des Brumes avant qu'elle engloutisse l'île.

---

## Conditions de fin de partie

### ✅ Victoire
Le joueur remporte la partie si :
1. Les **3 fragments** ont été récupérés (état = `obtenu`)
2. **L'Artefact est activé** lors du rituel de réunification (voir ci-dessous)

### ❌ Défaite
Le joueur perd la partie si :
- Ses **PV tombent à 0** (mort en combat ou piège fatal)
- Le **compteur de Tempête atteint 10** (voir section Tempête des Brumes)

---

## Suivi des fragments

| Fragment         | Zone                        | État          |
|------------------|-----------------------------|---------------|
| Fragment Sylvestre | Forêt des Hévalords (Nord) | Non découvert |
| Fragment Forgé   | Cité de Fer (Centre)        | Non découvert |
| Fragment des Brumes | Marais du Clergé (Sud)   | Non découvert |

### États possibles
- `Non découvert` — le joueur n'a pas encore exploré la zone
- `En cours` — le joueur est engagé dans le défi de la zone
- `Obtenu` — le fragment a été récupéré

---

## Conditions de récupération par fragment

### 🌿 Fragment Sylvestre — Forêt des Hévalords
**Gardien** : Ours Ombrefeu (boss de zone, PV = END × 4 = 32)
**Défi** : Résoudre l'Énigme de l'Arbre-Mémoire avant d'affronter le gardien.
- Si le joueur résout l'énigme → le gardien est affaibli (PV divisés par 2)
- Si le joueur échoue ou ignore l'énigme → combat en conditions normales
**Bonus d'alliance Hévalords** : Si le joueur est allié aux Hévalords, le gardien ne combat pas et remet le fragment librement.

### 🔥 Fragment Forgé — Cité de Fer
**Gardien** : Salamandre des Roches × 3 (défenseurs de l'ancienne forge)
**Défi** : Accéder à la forge magique oubliée nécessite un jet d'INT (1d10 ≤ INT) pour déchiffrer les mécanismes anciens.
- Succès → accès direct, un seul gardien actif
- Échec → les 3 gardiens s'éveillent
**Bonus d'alliance Cité de Fer** : Les gardes de la guilde indiquent l'emplacement exact (pas de jet d'INT requis).

### 🌫️ Fragment des Brumes — Marais du Clergé
**Gardien** : Sylphide de Brume + Loup Fantomatique (combat simultané)
**Défi** : Traverser les illusions du marais nécessite un jet de CHA (1d10 ≤ CHA) pour ne pas être égaré.
- Succès → chemin direct vers le fragment
- Échec → le joueur subit 1d3 dégâts d'épuisement et arrive affaibli au combat
**Bonus d'alliance Clergé des Brumes** : La Sylphide devient alliée et combat aux côtés du joueur.

---

## Rituel de réunification

Une fois les 3 fragments réunis, le joueur doit trouver le **Sanctuaire de l'Équilibre** (lieu neutre au centre de l'île, connu uniquement si au moins une faction est alliée).

**Jet de réunification** : 1d10 ≤ INT + bonus de faction (voir tableau)

| Factions alliées    | Bonus INT pour le rituel |
|---------------------|--------------------------|
| Aucune              | 0                        |
| 1 faction           | +1                       |
| 2 factions          | +2                       |
| 3 factions          | Succès automatique       |

- **Succès** → l'Artefact est réactivé, la Tempête des Brumes se dissipe → **Victoire**
- **Échec** → le rituel est perturbé, le compteur de Tempête augmente de 2, le joueur peut réessayer

---

## Compteur de Tempête des Brumes

La tempête progresse à chaque événement majeur. Elle représente l'urgence du scénario.

**Le compteur augmente de 1 à chaque fois que :**
- Le joueur échoue un défi de fragment (énigme ou jet raté)
- Le joueur perd un combat contre un boss de zone (et survit)
- Le joueur refuse d'agir lors d'un événement scénaristique important

**Le compteur augmente de 2 si :**
- Le rituel de réunification échoue
- Le joueur trahit une faction après alliance

**Le compteur diminue de 1 si :**
- Un fragment est obtenu avec succès
- Le joueur accomplit une action héroïque reconnue par une faction

| Compteur | Effet narratif                                              |
|----------|-------------------------------------------------------------|
| 1–3      | Tempêtes légères, visibilité réduite dans certaines zones   |
| 4–6      | Routes coupées, rencontres aléatoires plus fréquentes (+1 jet de rencontre) |
| 7–9      | Zones inaccessibles, PNJ hostiles, créatures plus agressives |
| 10       | La tempête engloutit l'île → **Défaite**                   |

---

## Conséquences narratives (fin de partie)

Le dénouement varie selon les alliances formées et les choix effectués pendant la quête.

| Situation à la victoire                        | Fin obtenue                                               |
|------------------------------------------------|-----------------------------------------------------------|
| 3 factions alliées                             | **Paix durable** — les factions unissent leurs forces    |
| 1 ou 2 factions alliées                        | **Équilibre fragile** — la faction alliée gagne en influence |
| Aucune faction alliée (quête en solitaire)     | **Victoire solitaire** — l'île est sauvée mais divisée   |
| Une faction trahie                             | **Paix instable** — tensions persistantes, risque de guerre |
| Artefact activé avec compteur Tempête ≥ 7     | **Victoire partielle** — l'île est sauvée mais endommagée |
