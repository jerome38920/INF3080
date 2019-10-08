##### Droits d'auteur :copyright: matériel protégé 
 - Si vous n'êtes pas un étudiant du cours INF3080-030 A2019 vous devez demander une permission pour l'utilisation de ce matériel.

# Séance 2: Modélisation conceptuelle, ssh, nano, sqlplus

- Objectif : Réfléchir et dessiner 
   + Secondaire : Augmenter notre niveau d'aisance avec l'environnement Linux

----
**Note** : (_facultatif_) S'il y a des questions dans ce labo, répondez y dans un fichier nommé
`./labo/reponse-labo.md`.  Le fichier doit être dans un format `Markdown`. Utilisez le projet
`in3080-a2019` pour déposer le fichier demandé. Utiliser le même fichier pour tous les exercices.

##### Format du fichier Markdown
 + Séance 2 (Header 1)
 + Exercice {1..n} (H2)
 + Question {1..n} (H4)
 + S`2`.E`3`.Q`1` (strong) `est une valeur qui change bien sûr`
 + La réponse dans une section script (code block)

**Note**: Il est recommandé de versionner vos réponses aux exercices à l'aide
de Git. Un seul dépôt est amplement suffisant pour tous les laboratoires, en
divisant les fichiers dans des répertoires.

 > > Pourquoi versionner vos exercices avec Git: afin de
vous entraîner à utiliser le logiciel (commandes) naturellement.

----


## 1 - Modélisation Conceptuelle

### 1a - module de connexion (login) d'une application Web

Vous devez dans cet exercice créer un modèle conceptuel qui existe dans tous les systèmes du monde.  Facebook, Twitter, Skype, gmail.

Il est probable que vous ayez à faire ceci plusieurs fois dans votre parcours professionnel.

Quelles sont les entités, attributs et les associations nécessaires pour obtenir un modèle simple et compréhensible pour une personne
comme l'enseignant du cours INF3080 A2019.  :wink:

Afin de rendre le tout un petit peu plus complet, j'aimerais que soit ajoutée la cardinalité entre les entités.

Utiliser la notation hongroise bien que celle-ci ne soit pas nécessaire dans un modèle conceptuel.  
Nous l'appellerons le modèle conceptuel enrichi.

Si vous désirez faire un diagramme de classes, c'est possible. Faites-le dans une deuxième passe de votre réflexion.

__Note__ : ne pas prendre plus de 15 minutes pour faire l'exercice. Si vous avez besoin de plus de temps pour finaliser, prendre une pause et revenir pour 5 minutes.

#### Questions:
+ Q1. Quelle est la difficulté ?
+ Q2. Avez vous réussi en moins de 15 minutes ?
+ Q3. Produire modèle dans un fichier.

### 1b - module de gestion d'une flotte de camions du style 53'

Maintenant que vous êtes bien échauffé, vous devez maintenant vous mettre dans la tête d'un
informaticien qui a un mandat pour modéliser une partie d'un système pour un transporteur 
majeur (Robert Transport, Guilbeault, Day & Ross).  Vous avez dû les voir sur les routes.

Votre rôle est de faire le modèle conceptuel pour la gestion d'une flotte de remorques + tracteurs (camions).
Vous devez savoir que les camions sont à un seul endroit dans le monde.  La latitude, longitude est utilisé
pour situer le camion sur la terre.

En plus de lister des camions, ce que nous voulons maintenir est combien coûte un camion qui roule. Deux états 
sont utiles pour le calcul: vide ou chargé (plein).  Vous venez de réaliser qu'une capacité de chargement est un
aspect important de ce domaine.  Vous savez aussi que les camions fonctionnent au pétrole, diesel (gazoualle) 
pour certains. Ils n'ont pas tous la même consommation. Les véhicules routiers sont identifiables, ont tous
une plaque et ont aussi besoin d'une assurance.

Encore, une fois gardez-le tout simple. Votre modèle conceptuel enrichi (MCE) contiendra l'information suivante :
entités, attributs, associations et sans oublié la cardinalité.

Bonne réflexion.

Notes :
 + utilisez une méthode itérative pour faire le travail.
 + ne pas utiliser word ou excel pour faire ce devoir.

#### Questions:
 + Q1. Rendre disponible votre modèle en format pdf ou autre. 

## 2 - ssh + nano + sqlplus
##### Contribution MT, UQAM

Une fois que vous avez réussi à vous connecter sur Oracle avec :
  - le script magique 
  - ou manuellement
  
et tout fonctionne, soyez fier. :relieved:

En revanche, une fois connecté sur Oracle, le shell fournit par Oracle est un peu arride (brutale) à l'utilisation 
et empêche de retourner en arrière (affiche les signes [[D^[[A^[[C^...etc). 

Je vous propose de rajouter la commande `rlwrap` avant de lancer `sqlplus`. 
Vous le connaissez peut-être déjà, mais `rlwrap` est un outil qui permet d'éditer une commande en utilisant la librairie readline de gnu. On peut ainsi revenir en arrière avec les flèches quand on a fait une faute et on peut aussi accéder à l'historique des commandes avec la flèche du haut (comme dans bash).

On peut soit utiliser `rlwrap` en lançant `sqlplus` comme mentionné dans le fichier `connection.md` :

```
rlwrap sqlplus <usager|codems>/<mot de passe>
```

Ou l'utiliser la commande avant de lancer le script :

```
rlwrap ./start.sh
```

Moi (MT) j'ai rajouté la commande rlwrap dans votre script et ça fonctionne bien :

```shell
#!/bin/bash
#GNU 3.0 Guy Francoeur 2018
p=$(grep -R ~/oracle.txt -e 'mot de passe: ' | cut -d\   -f4)
echo ${p}
l=$(grep -R ~/oracle.txt -e 'usager: ' | cut -d\   -f2)
echo ${l}
rlwrap sqlplus ${l}/${p}
```

----
Auteur :copyright: Guy Francoeur, version A2019
