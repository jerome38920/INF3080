# Connexion __Magique / Automatique__ à Oracle

## édition UQAM A2019

+ Le script suivant est rendu disponible afin de créer un fichier start.sh lequel vous lancerez pour connecter Oracle via SQLplus.
+ Copier et coller le code une seule fois pour créer le fichier start.sh.
+ Faire `CTRL-X` dans `nano` pour sortir et sauvegarder.

~~~~
$ nano start.sh
~~~~

### le script à copier dans `start.sh`
~~~~
#!/bin/bash
#GNU 3.0 Guy Francoeur 2018
p=$(grep -R ~/oracle.txt -e 'mot de passe: ' | cut -d\   -f4)
echo ${p}
l=$(grep -R ~/oracle.txt -e 'usager: ' | cut -d\   -f2)
echo ${l}
sqlplus ${l}/${p}
~~~~

### pour changer les droits
~~~~
$ chmod +x start.sh
~~~~

### pour lancer le script et entrer dans Oracle
~~~~
$ ./start.sh
~~~~

#### fin

---
Copyright :copyright: 2018 Guy Francoeur
