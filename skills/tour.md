# 🔄 Structure d'un Tour de Jeu — Verdhame

Ce fichier définit le déroulement obligatoire de chaque tour de jeu. Le Maître du Jeu doit respecter cet ordre à chaque interaction avec le joueur.

---

## Étape 1 — Narratif de la situation

Le MJ décrit la situation actuelle de façon immersive :
- L'environnement (lieu, ambiance, météo, brumes)
- Les personnages présents (PNJ, ennemis, alliés)
- Les éléments notables visibles ou perceptibles
- Si la **Vision des Brumes** est active, signaler toute embuscade ou piège détecté

> Le narratif doit refléter l'état actuel du joueur (PV, alliances, compteur de Tempête) et les conséquences des actions précédentes.

---

## Étape 2 — Réponse du joueur

Le joueur décrit librement son action. Le MJ ne doit pas contraindre les choix. Toute action est possible, même inattendue.

Si l'action est ambiguë, le MJ peut demander une clarification courte avant de résoudre.

---

## Étape 3 — Évaluation de la situation

Le MJ résout l'action selon les règles en vigueur :

### Résolution des jets de dés
- Identifier la caractéristique applicable (FOR / AGI / END / INT / CHA)
- Lancer 1d10 et comparer au seuil
- Appliquer les effets (succès, échec, critique, échec critique)
- Appliquer les règles de combat si nécessaire (→ voir skills/combat.md)

### Conséquences narratives
- Modifier les alliances si nécessaire (Neutre / Méfiant / Allié / Hostile)
- Ajuster le **compteur de Tempête** (+1 échec, -1 succès notable, +2 trahison)
- Attribuer les XP si un ennemi est vaincu (→ voir formule bestiaire)
- Vérifier si une montée de niveau est atteinte (XP ≥ niveau × 100)

---

## Étape 4 — Mise à jour de joueur.md

**Obligatoire après chaque tour.** Le MJ met à jour le fichier `memory/joueur.md` avec :

- ✅ PV actuels (après dégâts ou soins)
- ✅ XP gagné et total mis à jour
- ✅ Niveau si montée de niveau (+ ajustement des caractéristiques et PV max)
- ✅ Inventaire (objets gagnés ou perdus)
- ✅ Points de compétence disponibles
- ✅ Statut des alliances
- ✅ Compteur de Tempête
- ✅ État des fragments de quête
- ✅ Position actuelle du joueur
- ✅ Note de partie résumant l'action du tour

---

## Étape 5 — Validation des conditions de fin de partie

Avant de rendre la main au joueur, vérifier (→ voir skills/quete.md) :

### Victoire ?
- [ ] Les 3 fragments sont à l'état `Obtenu`
- [ ] Le rituel de réunification a été réussi

### Défaite ?
- [ ] PV du joueur = 0
- [ ] Compteur de Tempête = 10

### Fin de quête partielle ?
- [ ] Un fragment vient d'être obtenu → mettre à jour son état dans joueur.md

> Si une condition de fin est atteinte, le MJ annonce la fin de partie et décrit le dénouement narratif selon les alliances formées (→ tableau des conséquences dans skills/quete.md).

---

## Résumé visuel

```
[Narratif] → [Action joueur] → [Évaluation + jets] → [MAJ joueur.md] → [Vérif fin de partie] → [Narratif suivant]
```
