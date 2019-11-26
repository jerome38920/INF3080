##### Droits d'auteur :copyright: matériel protégé 
 Si vous n'êtes pas étudiant du cours INF3080-030 A2019 vous devez 
 - demander une permission pour l'utilisation de ce matériel;
 - fournir la raison de son usage;

# Séance 9: Sécurité, droits et synomyne 

- Objectif : Gèrer les droits sur des objets avec un usager en plus de simplifier l'usage des objets.

Vous avez 2 heures.
   
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

## 0 - Directives

+ Faites le maximum selon vos connaissances;
+ Lire l'atelier complètement;
+ Ce devoir utilise le schéma de base de données [modèle A](./modele_labo.png);
+ Je vais vérifier (lire) les devoirs;

![modèle A](./modele_labo.png)

## 1 - Donner des droits

 Vous devez donner des droits sur des tables de votre schéma à l'usager inf3080b. Utiliser une ou des tables du `modèle A`.

## 2 - Créer des synonymes

 ```bash
 # login/password
 inf3080b/GgbVKKxG
 ```

 Vous devez maintenant utiliser le schéma `inf3080b` et créer des synonymes pour les tables du #1. Ajouter
 votre codeMS dans le nom du synonyme. Une fois ceci fait vous devez créer une vue (view) nommée `v_codems`
 qui utilise les synonymes. Finalement, faire un SELECT sur la vue `v_codeMS`. LE CodeMS est bien sur votre codeMS, pas le mot codeMS.

 + Q1. Pourquoi ajouter le/votre `codeMS` au nom du synonyme ?

## 3 - Remettre tout comme avant !

 Vous devez créer un script nommé s09_n03.sql qui fera tout ce qui est nécessaire pour remettre le schéma 
 `inf3080b` dans l'état initial.  Vous ne devez pas effacer les objets de vos collègues.  Vous devez aussi
 en utilisant le même script enlever les droits initialement donnés.

## 4 - SQL*loader

Dans la table `Historique` déjà créer vous devez importer les données ci-bas.
Les domaines de champs (colonne) sont détectables à l'aide de la notation hongroise et des valeur proposées.
Vous remarquez que les colonnes date sont étrange, ouille des fois c'est pas beau. Rien n'est à votre épreuve. 


| pHistorique | dCreation | dExpiration | cIP | pLangue |
| ----------- | ---------- | ----------- | ---- | ----- |
| 10         | 30-2019-01 | 01-2019-30 | 192.168.1.100 | 2 | 
| 20         | 28-2018-12 | 12-2018-29 | 192.168.2.200 | 3 |
| 31         | 15-2017-12 | 12-2017-16 | 192.168.3.254 | 4 |

### Questions :

 + Q2.  Quelles sont les commandes qui permettent de changer d'usager sans fermer SQL*plus ?
 + Q3.  Pourquoi est-ce utile de créer des synomymes ? ou dans quel cas (élaborer-le) ?
 + Q4.  Lorsque nous travaillons avec un outils d'import comme SQL*loader que devons-vous garder en tête ?
 + Q5.  Combien de temps a été nécessaire pour faire l'atelier ?

### FIN.

---

Auteur Guy Francoeur :copyright: version A2019
