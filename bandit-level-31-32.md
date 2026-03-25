# Bandit Level 31 → 32

## Objectif
Pousser un fichier vers un repo git distant pour 
récupérer le mot de passe.

## Commandes utilisées
git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo
cd repo
cat README.md
echo "May I come in?" > key.txt
git add -f key.txt
git commit -m "add key.txt"
git push origin master

## Ce que j'ai appris
- git push envoie des commits vers un repo distant
- -f force l'ajout d'un fichier ignoré par .gitignore
- Le serveur peut exécuter des actions lors d'un push (git hooks)
- Concept clé : git hooks et push vers remote
