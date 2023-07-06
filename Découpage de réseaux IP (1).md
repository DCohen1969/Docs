# Découpage de réseaux IP
#
**Le réseau est 172.16.1.0/24** 
#
##### Avec X nombre de machines:
#
**La formule pour calculer le nombre de bits hôte:**
on obtien en  **2^n-1 < X < 2^n**, n soit la puissance de 2 qui est immediactement superieur à X.  

**La formule pour le nombre de machines addressable:**
**2 ^ (nbre bits hôte) - 2**

donc:
 
**nbre bits hôte** = 32 – 24 = 8

alors: 
 2 ^ (8) – 2 = 254


**Nous pouvons donc adresser 50  dans le premier reseaux, ce qui donne:**
**2^5 < 50 < 2^6** donc on prends le 6 pour la formule donc **32 - 6** ce qui donne **26**

**Nous pouvons donc adresser 12  dans le premier reseaux, ce qui donne:**
**2^3 < 12 < 2^4** donc on prends le 4 pour la formule donc **32 - 4** ce qui donne **28**

**Nous pouvons donc adresser 20  dans le premier reseaux, ce qui donne:**
**2^4< 20 < 2^5** donc on prends le 5 pour la formule donc **32 - 5** ce qui donne **27**

**Nous pouvons donc adresser 15  dans le premier reseaux, ce qui donne:**
**2^8< 15 < 2^4** donc on prends le 4 pour la formule donc **32 - 4** ce qui donne **28**

![Le tableau]('https://github.com/DCohen1969/Docs/blob/main/D%C3%A9coupage%20de%20r%C3%A9seaux%20IP%20-%20resultat.jpg')


