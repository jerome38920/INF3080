##### Droits d'auteur :copyright: matériel protégé 
 Si vous n'êtes pas étudiant du cours INF3080-030 A2019 vous devez 
 - demander une permission pour l'utilisation de ce matériel;
 - fournir la raison de son usage;

# Séance 7: Langage SQL - DDL, DML, TCL

- Objectif : Expérimenter le DDL, DML, TCL
   
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
+ Ce devoir est la suite du devoir précédent;
+ Débuter le devoir;
+ Je vais vérifier (lire) les devoirs;

## 1 - Création de requêtes SQL pour Oracle

Vous devez créer un script  nommé `labo07.sql` qui qui contiendra les réponses pour toutes les questions qui suivent.
Vous devez pour ce travail utiliser le schéma de base de données [modèle A](./modele_labo.png). Les modifications sont
incrémentales.

![modèle A](./modele_labo.png)

+ a) Assurez-vous d'avoir des tuples dans chacune des tables (environ 7+);
+ b) Il faut sauvegarder vos changements dans la BD;
+ c) Écrire une requête qui efface la plus petite pLangue qui n'est pas dans une relation (qui n'est pas une clé étrangère);
+ d) Écrire une requête qui crée un index unique sur le courriel afin de valider que le courriel est unique;
+ e) Écrire une requête qui modifie les tuples impairs de la table en ajoutant '(impair)' à Usager(cUsager); 
+ f) Écrire une requête qui liste le nombre de tuples (Historique) par cIP et cLangue ordonné par cLangue;
+ g) Écrire une requete qui change les mots de passe qui ont moins de 8 caractères vers un mot de 8 ou plus caractères;
+ h) Écrire une requête qui ajoute une règle qui invalide les cPassword de moins de 8 caractères; 
+ i) Écrire une requête qui ajoute un tuples dans Connexion avec moins de 8 caratères;
+ j) Lister le nombre de tuples avec moins 7 caratères UNION le nombre de typles avec 8 caractères Connexion(cPassword);
+ h) Saugarger vos tuples et votre script.

## 2 - Exécution de votre script

+ Q1. Comment est-ce possible d'exécuter un script dans SQL*plus ?

### FIN.

---

Auteur Guy Francoeur :copyright: version A2019
