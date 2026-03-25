# Bandit Level 30 → 31

## Objectif
Trouver le mot de passe du niveau suivant dans un dépôt git en utilisant des objets git (blobs) cachés.

## Commandes utilisées
git clone ssh://bandit30-git@bandit.labs.overthewire.org:2220/home/bandit30-git/repo
cd repo
git fsck --full
git show <blob-hash>

## Ce que j'ai appris
- git fsck --full permet de trouver tous les objets git, même ceux non référencés
- Les mots de passe peuvent être cachés dans des blobs ou des tags, pas forcément dans les fichiers visibles
- git show <hash> permet de lire le contenu d'un blob ou d'un objet git
- Importance de vérifier les tags et branches distantes
- Concept clé : exploration approfondie de l’historique git et des objets
