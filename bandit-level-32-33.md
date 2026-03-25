# Bandit Level 32 → 33

## Objectif
Échapper à un shell qui convertit tout en majuscules.

## Commandes utilisées
$0
whoami
cat /etc/bandit_pass/bandit33

## Ce que j'ai appris
- Le uppercase shell convertit toutes les entrées en majuscules
- Les commandes Linux en majuscules ne sont pas reconnues
- $0 est une variable spéciale qui référence le shell actuel
- $0 n'est pas affecté par la conversion en majuscules
- Une fois dans bash via $0, on peut exécuter des commandes normalement
- Concept clé : escape de shell restrictif avec variables spéciales
