# Bandit Level 4 → 5

## Objectif
Trouver le seul fichier lisible parmi 10 fichiers.

## Commandes utilisées
ls
cd inhere
ls -la
file ./*
cat ./-file07

## Ce que j'ai appris
- La commande file permet d'identifier le type de chaque fichier
- ./* cible tous les fichiers du dossier actuel
- Seul le fichier ASCII text contient du texte lisible
- Les autres fichiers contiennent des données binaires
