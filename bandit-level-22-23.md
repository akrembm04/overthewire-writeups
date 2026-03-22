# Bandit Level 22 → 23

## Objectif
Analyser un script cron qui génère un nom de fichier 
basé sur un hash MD5.

## Commandes utilisées
cat /etc/cron.d/cronjob_bandit23
cat /usr/bin/cronjob_bandit23.sh
echo I am user bandit23 | md5sum | cut -d ' ' -f 1
cat /tmp/8ca319486bfbbc3663ea0fbe81326349

## Ce que j'ai appris
- md5sum génère un hash MD5 d'une chaîne de texte
- cut -d ' ' -f 1 extrait le premier champ
- On peut simuler un script pour prédire son comportement
- Les noms de fichiers peuvent être générés dynamiquement
