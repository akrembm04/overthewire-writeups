# Bandit Level 25 → 26

## Objectif
Se connecter en bandit26 dont le shell est "more" 
au lieu de bash.

## Commandes utilisées
# Sur PowerShell :
scp -P 2220 bandit25@bandit.labs.overthewire.org:~/bandit26.sshkey C:\Users\mongia\bandit26.key
icacls C:\Users\mongia\bandit26.key /inheritance:r
icacls C:\Users\mongia\bandit26.key /grant:r mongia:R
# Réduire la fenêtre à 3 lignes de hauteur
ssh -i C:\Users\mongia\bandit26.key bandit26@bandit.labs.overthewire.org -p 2220
# Dans more : appuyer sur v pour ouvrir vim
:set shell=/bin/bash
:shell

## Ce que j'ai appris
- Le shell d'un utilisateur peut être autre chose que bash
- more se met en pause si la fenêtre est trop petite
- vim peut ouvrir un shell avec :shell
- On peut changer le shell dans vim avec :set shell=
