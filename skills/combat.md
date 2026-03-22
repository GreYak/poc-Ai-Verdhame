# ⚔️ Règles de Combat — Île de Verdhame

## Structure d'un tour

1. **Initiative** — Jet de 1d10 + AGI pour chaque combattant → le plus haut agit en premier
2. **Attaque** — L'attaquant choisit son type d'attaque et effectue un jet
3. **Réponse** — La cible choisit de **résister** ou **esquiver**
4. On passe au combattant suivant, jusqu'à ce qu'un camp atteigne 0 PV

---

## Jet d'attaque (1d10)

Lancer 1d10. Si le résultat est **≤ à la caractéristique utilisée → Touché**.

| Type d'attaque           | Caractéristique utilisée |
|--------------------------|--------------------------|
| Corps à corps            | FOR                      |
| Agile / Furtive / Arc    | AGI                      |
| Magique                  | INT                      |
| Intimidation / Manipulation | CHA                   |

- **Critique** : résultat = 1 → dégâts ×2
- **Échec critique** : résultat = 10 → l'attaquant subit 1 dégât (maladresse)

---

## Calcul des dégâts

**Dégâts = caractéristique d'attaque ÷ 2** (arrondi au supérieur, minimum 1)

| Caractéristique | Dégâts de base |
|-----------------|----------------|
| 1–2             | 1              |
| 3–4             | 2              |
| 5–6             | 3              |
| 7–8             | 4              |
| 9–10            | 5              |

---

## Défense — la cible choisit

- **Résister** : réduction = END ÷ 3 (arrondi inférieur, minimum 0)
  - Dégâts finaux = Dégâts − réduction (minimum 1)
- **Esquiver** : jet 1d10 ≤ AGI → aucun dégât ; échec → dégâts en plein (sans réduction)

> L'esquive est plus risquée mais potentiellement plus efficace pour les personnages à forte AGI.

---

## PV des créatures

- **Créature commune** (Faune, Nuisible, Prédateur, Marin) : **PV = END × 2**
- **Créature rare / Boss** (Mystique, Golem, Dragon, Kraken) : **PV = END × 4**

| Créature            | Type     | END | PV  |
|---------------------|----------|-----|-----|
| Grillon Géant       | Nuisible | 2   | 4   |
| Loup des Brumes     | Faune    | 5   | 10  |
| Sanglier Rugissant  | Prédateur| 6   | 12  |
| Serpent d'Obsidienne| Prédateur| 5   | 10  |
| Ours Ombrefeu       | Prédateur| 8   | 16  |
| Golem des Ruines    | Mystique | 10  | 40  |
| Dragon des Brumes   | Mystique | 10  | 40  |
| Kraken de Verdhame  | Marin    | 10  | 40  |

---

## Compétences en combat

- Chaque utilisation de compétence **remplace ou amplifie l'action du tour**
- Nécessite d'avoir débloqué la compétence (points de compétence dépensés lors de la progression)
- Les effets de zone ou de contrôle sont limités à leur durée définie dans l'arbre de compétences
- Pas de limite d'utilisation par combat

---

## Fin du combat

- **Créature à 0 PV** → vaincue ; XP calculé selon la formule du bestiaire :
  `XP = EXP_base × (1 + (Niveau créature − Niveau joueur) / 5) × (0.8 + 0.4 × Random)`
- **Joueur à 0 PV** → incapacité (fin de partie, ou sauvetage scénaristique selon contexte)
