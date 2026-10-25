<h1 align="center">🎲 Dominos vs AI</h1>

<p align="center"><em>28 dominos, 7 pour chacun, et un adversaire qui calcule ses coups. Sauras-tu le battre ?</em></p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python 3" />
  <img src="https://img.shields.io/badge/d%C3%A9pendances-aucune-success?style=for-the-badge" alt="Aucune dépendance" />
  <img src="https://img.shields.io/badge/projet%20d%27apprentissage-ff69b4?style=for-the-badge" alt="Projet d'apprentissage" />
</p>

---

## ✨ Pourquoi tu vas l'adorer

- **Un vrai jeu de dominos** : la chaîne grandit des deux côtés, et tu peux piocher au talon.
- **Une IA qui réfléchit** : elle joue le domino dont les valeurs sont les plus présentes sur la table et dans sa main.
- **Un écran lisible** à chaque tour : talon, nombre de dominos de l'ordinateur, chaîne et tes dominos numérotés.

## 📜 Règles

- Les 28 dominos sont mélangés : 7 pour toi, 7 pour l'ordinateur, 14 au talon.
- Celui qui possède le plus gros double commence.
- Gagne celui qui vide sa main en premier.

## 🎮 Commandes

| Saisie | Effet |
|:---:|---|
| `3` | Pose ton 3e domino à droite de la chaîne, si la valeur correspond |
| `-2` | Pose ton 2e domino à gauche, si la valeur correspond |
| `0` | Pioche un domino au talon |

## 🚀 Lancer

```bash
python3 dominoes.py
```

## 🕹️ Exemple d'écran

Les dominos changent à chaque partie ; voici la structure de l'écran au premier tour :

```text
======================================================================
Stock size: 14
Computer pieces: 6

[6, 6]
Your pieces:
1: [1, 4]
2: [0, 3]
...

Status: It's your turn to make a move. Enter your command.
```

## 🧠 Sous le capot

- `who_start()` compare les doubles des deux joueurs pour désigner le premier.
- `domino_counter()` compte les valeurs présentes sur la table et dans la main de l'IA : c'est la base de son score.
- `snake_printer()` raccourcit l'affichage (début et fin seulement) dès que la chaîne dépasse six dominos.

## 🔭 Pistes d'évolution

- Corriger la détection du match nul : la condition actuelle ne peut jamais être vraie.
- Gérer le cas où aucun joueur n'a de double au départ, situation qui fait planter le programme aujourd'hui.

---

<p align="center"><sub>Fait avec ❤️ et Python par DSKarim</sub></p>
