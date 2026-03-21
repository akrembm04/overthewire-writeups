# Bandit Level 12 → 13

## Objectif
Retrouver le mot de passe dans un fichier compressé 
plusieurs fois de suite (hexdump).

## Commandes utilisées
mkdir /tmp/mywork12
cp ~/data.txt /tmp/mywork12/
cd /tmp/mywork12
xxd -r data.txt > data.bin
mv data.bin data2.gz && gunzip data2.gz
mv data2 data2.bz2 && bunzip2 data2.bz2
mv data2 data4.gz && gunzip data4.gz
tar xf data4
tar xf data5.bin
mv data6.bin data6.bz2 && bunzip2 data6.bz2
tar xf data6
mv data8.bin data8.gz && gunzip data8.gz
cat data8

## Ce que j'ai appris
- xxd -r convertit un hexdump en fichier binaire
- file identifie le type de compression
- gzip, bzip2, et tar sont des formats de compression courants
- Il faut décompresser couche par couche
- mv + extension correcte avant de décompresser
