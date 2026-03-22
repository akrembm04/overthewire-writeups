# Bandit Level 21 → 22

## Objectif
Trouver le mot de passe généré par un cron job.

## Commandes utilisées
ls /etc/cron.d/
cat /etc/cron.d/cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

## Ce que j'ai appris
- Les cron jobs sont des tâches planifiées automatiques
- /etc/cron.d/ contient les configurations des cron jobs
- Un script peut copier des données sensibles dans /tmp
- Analyser les scripts cron peut révéler des informations critiques
