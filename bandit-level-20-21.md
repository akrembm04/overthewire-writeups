# Bandit Level 20 → 21

## Objectif
Utiliser suconnect pour récupérer le mot de passe 
en écoutant sur un port local.

## Commandes utilisées
echo "Password" | nc -lp 1234 &
./suconnect 1234

## Ce que j'ai appris
- nc -lp ouvre un listener sur un port
- & exécute la commande en arrière-plan
- suconnect se connecte au port et vérifie le mot de passe
- Si correct, il retourne le mot de passe du niveau suivant
- Concept fondamental : communication entre processus via ports
