# Bandit Level 19 → 20

## Objectif
Utiliser un binaire setuid pour lire le mot de passe 
de bandit20.

## Commandes utilisées
ls
./bandit20-do cat /etc/bandit_pass/bandit20

## Ce que j'ai appris
- Un fichier setuid s'exécute avec les permissions de son propriétaire
- bandit20-do appartient à bandit20 → il peut lire ses fichiers
- Les binaires setuid sont une surface d'attaque importante en cyber
- C'est la base de l'escalade de privilèges Linux
