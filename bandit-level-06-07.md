# Bandit Level 6 → 7

## Objectif
Trouver un fichier quelque part sur le serveur 
avec des propriétés spécifiques.

## Commandes utilisées
find / -type f -size 33c -user bandit7 -group bandit6 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password

## Ce que j'ai appris
- find / cherche depuis la racine du système entier
- -user et -group filtrent par propriétaire
- 2>/dev/null cache les erreurs "Permission denied"
- Sans 2>/dev/null les erreurs noient les résultats
