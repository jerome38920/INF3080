##### Droits d'auteur :copyright: matériel protégé 
 Si vous n'êtes pas étudiant du cours INF3080-030 A2019 vous devez 
 - demander une permission pour l'utilisation de ce matériel;
 - fournir la raison de son usage;

# Séance 4: Langage SQL

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
+ Lire l'atelier completement;
+ Débuter le devoir;

## 1 - Création de vues (view)

Vous devez créer des vues qui nous aideront à lister les objets contenus dans votre schéma (lié à
votre identifiant). Coder les réponses dans un script nommé `01_systeme.sql`.

+ a) lister les tables dans v_tables(nom);
+ b) lister les tables et les vues dans v_objets(nom, type);
+ c)  modifier v_tables afin d'ajouter le nombre de lignes (tuples) de la table;
+ d) Quel est le prérequis pour obtenir le nombre de tuples;

## 2 - Creation du modèle de gestion des accès

Vous devez créer le schéma à partir du modèle relationnel [modèle A](./modele.png).  Votre script
sera nommé `02_schema.sql`.

+ a) Créer les tables avec les attributs;
+ b) Ne pas ajouter les clés à ce moment;

## 3 - Insertion de données

Vous devez créer un fichier nommé `03_insert.sql` qui ajoute pour chacune des tables, au moins 3 tuples.

## 4 - Modification du schéma

Vous devez ajouter les clés primaires pour chacune des tables à l'aide de la commande ALTER TABLE. Vos
commandes seront ajoutées au fichier `04_alter.sql`.

+ a) faites les ajouts de clés;
+ b) ajouter au moins 1 enregistrement dans chacune des tables;

## 5 - Validation (test)

Assurez-vous que tous vos fichiers sont complets et bien sauvegardés. Vous devez fermer toutes vos 
sessions SQL*plus. Relancer SQL*plus.  Par la suite, vous devez valider que les tables ont le nombre
de lignes en fonction des insertions.  Est-ce que vos vues sont toujours valides?  Avez-vous des 
problèmes avec vos objets? Tous vos tests seront codés et sauvegardés dans un fichier nommé 
`05_test.sql`.

## 6 Exécution totale

Vous devez exécuter tous les scripts que vous avez créés.  Ils devront être exécutés dans l'ordre
au moins deux fois.  Vous ne devez pas avoir d'erreur à la suite des deux exécutions successives.

### FIN.

---

Auteur Guy Francoeur :copyright: version A2019
