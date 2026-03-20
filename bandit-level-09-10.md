# Bandit Level 9 → 10

## Objectif
Trouver le mot de passe dans un fichier binaire,
précédé de plusieurs "=".

## Commandes utilisées
ls
strings data.txt | grep "==="

## Ce que j'ai appris
- strings extrait les textes lisibles d'un fichier binaire
- grep "===" filtre les lignes contenant ===
- Combinaison puissante pour chercher dans des fichiers binaires
