# **Installation de Wireshark et analyse de trames ethernet**

# Les questions:
#
##### **1**.Quels protocoles ont été utilisés dans la trace réseau capturée ? Indique comment tu as eu cette information (quelle fenêtre, éventuellement quelle ligne ou quelle colonne).

**Protocoles:**
* ARP (fênetre liste des paquets - Colonne: Protocol - Lignes: 1,2)
* ICMP (fênetre liste des paquets - Colonne: Protocol - Lignes: 3 à 10)

#
##### **2**.Quelles sont les adresses IP et les adresses MAC des interfaces ayant échangé des information ?

**Paquet Nº 1** 
* Sender MAC address: Private_66:68:00 **(00:50:79:66:68:00)**
* Target MAC address: Broadcast **(ff:ff:ff:ff:ff:ff)**

**Paquet Nº 2** 
* Sender MAC address: Private_66:68:01 **(00:50:79:66:68:01)**
* Target MAC address: Private_66:68:00 **(00:50:79:66:68:00)**

#
##### **3**.Quel filtre d'affichage permet de ne plus afficher les paquets ARP ?
* **“not arp”**
#
##### **4**.Quelle information sont disponible dans la colonne info de la liste des paquets pour la ligne 3 ?
C'est une question ou requête ping:
* ICMP Type: 8 (Echo (ping) request)

##### **5**.Le paquet N°8 est-il une question ou une réponse ? et quel est le paquet correspondant (la question, si c'est une réponse ou la réponse, si c'est une question ?

Le paquet N°8 est une réponse au paquet Nº 7

* **Requête:**  Echo (ping) request  id=0xb98e, seq=3/768, ttl=64 (reply in 8)
* **Réponse:** Echo (ping) reply    id=0xb98e, seq=3/768, ttl=64 (request in 7)




