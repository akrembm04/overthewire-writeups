# Bandit Level 18 → 19

## Objectif
Lire un fichier malgré un .bashrc modifié qui 
déconnecte immédiatement.

## Commandes utilisées
ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"

## Ce que j'ai appris
- Le .bashrc s'exécute à chaque connexion SSH interactive
- On peut passer une commande directement à SSH sans ouvrir un shell
- Syntaxe : ssh user@host "commande"
- Technique utile pour contourner des restrictions shell
