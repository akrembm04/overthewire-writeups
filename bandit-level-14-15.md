# Bandit Level 14 → 15

## Objectif
Envoyer le mot de passe actuel sur le port 30000 de localhost.

## Commandes utilisées
cat /etc/bandit_pass/bandit14
echo "mot_de_passe" | nc localhost 30000

## Ce que j'ai appris
- nc (netcat) permet de se connecter à un port réseau
- On peut envoyer du texte via nc avec echo et pipe
- Les services réseau écoutent sur des ports spécifiques
- Netcat est un outil fondamental en cybersécurité
