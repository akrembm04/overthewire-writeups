# Bandit Level 11 → 12

## Objectif
Décoder un fichier encodé en ROT13.

## Commandes utilisées
ls
cat data.txt
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

## Ce que j'ai appris
- ROT13 est un chiffrement simple qui décale les lettres de 13 positions
- La commande tr permet de remplacer des caractères
- ROT13 est souvent utilisé en CTF et cybersécurité basique
- Appliquer ROT13 deux fois redonne le texte original
