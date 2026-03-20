# Bandit Level 5 → 6

## Objectif
Trouver un fichier avec des propriétés spécifiques 
parmi 20 dossiers.

## Commandes utilisées
ls
cd inhere
find . -type f -size 1033c ! -executable
cat ./maybehere07/.file2

## Ce que j'ai appris
- La commande find permet de chercher avec des critères précis
- -type f cible uniquement les fichiers
- -size 1033c filtre par taille exacte en bytes
- ! -executable exclut les fichiers exécutables
