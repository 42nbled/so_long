# so_long

## 🎮 À propos

Ce projet consiste à créer un jeu en 2D à l'aide de la MiniLibX, où le joueur doit collecter tous les objets présents sur une carte pour ensuite atteindre la sortie.

- Déplacements : W, A, S, D (ou Z, Q, S, D)
- Affichage du nombre de mouvements dans le terminal
- Fermeture propre via `ESC` ou la croix de la fenêtre

## 🛠️ Dépendances

- MiniLibX

## 🗺️ Carte

Le jeu prend en entrée une carte `.ber` décrivant le terrain avec :
- `1` : mur
- `0` : sol
- `C` : objet à collecter
- `E` : sortie
- `P` : position initiale du joueur

La carte doit être fermée par des murs, rectangulaire, et contenir au minimum :
- 1 sortie
- 1 joueur
- 1 objet à collecter

Exemple :
```
11111
1P0C1
100E1
11111
```

## 🛠️ Compilation

```bash
make
```

## 🚀 Lancement

```bash
./so_long maps/map.ber
```

## 📁 Structure attendue

- `maps/` : cartes `.ber`
- `textures/` : fichiers xpm pour les sprites
- `srcs/`, `includes/`, `Makefile`

## ❌ Pas inclus

- Pas de mouvements d’ennemis
- Pas d’animations ni affichage des déplacements à l’écran

## 🧼 Quitter proprement

Appuie sur `ESC` ou ferme la fenêtre pour quitter le jeu proprement.

---

> Projet réalisé dans le cadre du cursus 42 – Graphismes 2D avec MiniLibX.
