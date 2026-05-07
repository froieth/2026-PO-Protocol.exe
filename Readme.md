# Protocol.exe

## Présentation

**Protocol.exe** est un jeu de stratégie à deux joueurs inspiré des échecs et de l’univers de la cybersécurité.

Le jeu mélange :
- déplacements tactiques,
- gestion de cartes,
- commandes Linux,
- contrôle du plateau,
- stratégie rapide.

Les parties durent environ **5 à 10 minutes** et se jouent sur un plateau de **7 × 10 cases**.

---

# Objectif du jeu

Le but est de :
> atteindre le serveur adverse.

Chaque joueur possède un serveur placé à l’extrémité opposée du plateau.

Le premier joueur qui atteint le serveur ennemi :
# GAGNE LA PARTIE

---

# Plateau

- Taille : **7 colonnes × 10 lignes**
- Jeu : **2 joueurs**
- Le serveur est placé en dehors du plateau
- Chaque joueur possède 14 pions

---

# Début de partie

## Distribution des cartes

Chaque joueur :
- pioche **3 cartes** au hasard.

---

## Premier joueur

Une pièce est lancée :
- pile → Joueur 1 commence
- face → Joueur 2 commence

---

# Placement des pions

Les pions sont placés sur deux lignes.

## Première ligne

```txt
P P P D P P P
```

| Symbole | Pion |
|----------|------|
| P | Processus |
| D | DDOS |

---

## Deuxième ligne

```txt
M A V S F A M
```

| Symbole | Pion |
|----------|------|
| M | Mail Fishing |
| A | Antivirus |
| V | Virus |
| S | SQLI |
| F | Firewall |

---

# Déroulement d’un tour

## 1. Pioche

Au début de son tour :
- le joueur pioche une carte
- uniquement s’il possède moins de 5 cartes.

Main maximum :
> 5 cartes

---

## 2. Action

Le joueur doit choisir UNE seule action :

### Soit :
- déplacer un pion

### Soit :
- jouer une carte

---

## 3. Fin du tour

Une fois l’action terminée :
- le tour passe au joueur suivant.

---

# Les Pions

## Processus

Pion de base.

- avance d’une case
- capture en diagonale

---

## Daemon

Upgrade du Processus.

- déplacement d’une case dans toutes les directions

---

## Rootkit

Pion offensif.

- avance de deux cases en ligne droite
- saute les autres pions

---

## Firewall

Pion défensif.

- déplacement horizontal uniquement
- peut bloquer plusieurs cases du plateau pendant quelques tours

---

## DDOS

Pion perturbateur.

Lorsqu’il élimine un pion :
- 1 chance sur 2 de faire perdre le prochain tour adverse

---

## Virus

Meurt lorsqu'il tue un ennemi

- infecte les pions adjacents
- l’infection se propage une seule fois
- les pions infectés disparaissent après quelques tours

---

## Mail Fishing

Pion mobile inspiré du cavalier.

- déplacement en L
- saute les autres pions

---

## SQLI

Pion à distance.

- peut lancer des attaques SQL
- attaque à portée limitée

---

## Antivirus

Pion support.

- soigne les unités infectées
- peut nettoyer une zone infectée
- Meurt après avoir soigner les unité infectée

---

# Les Cartes Commandes

Les commandes Linux sont utilisées sous forme de cartes.

Les joueurs peuvent jouer une seule carte par tour.

---

## Liste des cartes

| Carte | Effet |
|--------|--------|
| `remove` | Supprime un pion adverse ciblé |
| `save` | Sauvegarde les positions et types des pions |
| `rollback` | Revient à la dernière sauvegarde |
| `chown` | Change le propriétaire d’un pion adverse adjacent |
| `exit` | Abandonne la partie |
| `create` | Crée un nouveau Processus |
| `upgrade` | Améliore un pion (Processus → Daemon → Rootkit) |
| `cp` | Duplique un pion allié |

---

# Résumé

Protocol.exe est un jeu d’échecs modernisé dans un univers informatique où :
- chaque déplacement compte,
- chaque commande peut changer la partie,
- et la moindre ouverture peut mener directement au serveur adverse.

