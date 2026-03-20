# Bandit Level 8 → 9

## Objectif
Trouver la seule ligne unique dans un fichier 
contenant beaucoup de lignes dupliquées.

## Commandes utilisées
ls
sort data.txt | uniq -u

## Ce que j'ai appris
- sort trie les lignes d'un fichier
- uniq -u affiche uniquement les lignes uniques
- Le pipe | envoie la sortie d'une commande vers une autre
- sort est nécessaire avant uniq pour que ça fonctionne
