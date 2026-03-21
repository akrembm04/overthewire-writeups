# Bandit Level 16 → 17

## Objectif
Scanner les ports 31000-32000, trouver le port SSL
et récupérer une clé SSH privée.

## Commandes utilisées
nmap -sV -p 31000-32000 localhost
echo "Password" | openssl s_client -connect localhost:31790 -quiet 2>/dev/null > /tmp/b17/key
# Sur PowerShell :
scp -P 2220 bandit16@bandit.labs.overthewire.org:/tmp/b17/key C:\Users\Wanted\bandit17.key
icacls C:\Users\Wanted\bandit17.key /inheritance:r
icacls C:\Users\Wanted\bandit17.key /grant:r Wanted:R
ssh -i C:\Users\Wanted\bandit17.key bandit17@bandit.labs.overthewire.org -p 2220

## Ce que j'ai appris
- nmap scanne les ports et identifie les services
- -sV détecte les versions des services
- Deux ports SSL trouvés : 31518 (echo) et 31790 (cible)
- Le serveur retourne une clé SSH au lieu d'un mot de passe
- SCP + icacls pour gérer la clé sur Windows
