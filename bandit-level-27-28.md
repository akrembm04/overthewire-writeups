# Bandit Level 27 → 28

## Objectif
Cloner un repo git et trouver le mot de passe dans README.

## Commandes utilisées
mkdir /tmp/b27 && cd /tmp/b27
git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo
cat repo/README

## Ce que j'ai appris
- git clone récupère un repo distant
- Les repos git peuvent contenir des informations sensibles
- Toujours vérifier le README en premier
- SSH avec port personnalisé dans une URL git : ssh://user@host:port/path
