# Bandit Level 28 → 29

## Objectif
Trouver un mot de passe supprimé dans l'historique git.

## Commandes utilisées
git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo
cd repo
git log
git show <commit-hash>

## Ce que j'ai appris
- git log affiche l'historique des commits
- git show affiche les changements d'un commit spécifique
- Les données supprimées restent dans l'historique git
- Ne jamais committer des mots de passe même temporairement
- Concept clé : forensics git
