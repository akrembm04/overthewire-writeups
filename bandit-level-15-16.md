# Bandit Level 15 → 16

## Objectif
Envoyer le mot de passe sur le port 30001 via SSL/TLS.

## Commandes utilisées
echo "Password" | openssl s_client -connect localhost:30001 -quiet

## Ce que j'ai appris
- SSL/TLS chiffre les communications réseau
- openssl s_client permet de se connecter à un service SSL
- -quiet réduit les messages de debug
- La différence entre nc (non chiffré) et openssl (chiffré)
