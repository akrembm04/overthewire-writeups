# Bandit Level 29 → 30

## Objectif
Trouver un mot de passe dans une branche git cachée.

## Commandes utilisées
git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo
cd repo
git branch -a
git show origin/dev:README.md

## Ce que j'ai appris
- git branch -a affiche toutes les branches locales et distantes
- Les branches distantes peuvent contenir des infos sensibles
- git show branch:fichier affiche un fichier dans une branche
- Ne pas se limiter à la branche main/master
- Concept clé : exploration des branches git
