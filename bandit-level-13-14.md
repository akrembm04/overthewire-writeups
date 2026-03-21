# Bandit Level 13 → 14

## Objectif
Se connecter en bandit14 en utilisant une clé SSH privée 
au lieu d'un mot de passe.

## Commandes utilisées
# Sur le serveur bandit13 :
ls
cat sshkey.private

# Sur PowerShell Windows :
scp -P 2220 bandit13@bandit.labs.overthewire.org:~/sshkey.private C:\Users\Wanted\bandit14.key
icacls C:\Users\Wanted\bandit14.key /inheritance:r
icacls C:\Users\Wanted\bandit14.key /grant:r Wanted:R
ssh -i C:\Users\Wanted\bandit14.key bandit14@bandit.labs.overthewire.org -p 2220
cat /etc/bandit_pass/bandit14

## Ce que j'ai appris
- Une clé SSH privée remplace le mot de passe
- SCP permet de copier des fichiers depuis un serveur distant
- Les permissions Windows doivent être restreintes pour que SSH accepte la clé
- chmod 600 sur Linux = icacls /inheritance:r sur Windows
