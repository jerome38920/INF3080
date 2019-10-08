##### Droits d'auteur :copyright: matériel protégé 
 Si vous n'êtes pas étudiant du cours INF3080-030 A2019 vous devez 
 - demander une permission pour l'utilisation de ce matériel;
 - fournir la raison de son usage;

# Séance 4: Algèbre relationnelle

- Objectif : Expérimenter l'algèbre relationnelle 
   
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

## 1 - module de ~~connexion~~ gestion des accès d'une application Web

Dans cette séance nous allons un peu plus loin.  Vous allez créer des requêtes 
en utilisant l'algèbre relationnelle et le modèle relationnel qui suit.

[modele](./modele.png)


#### Langue (données)

| pLangue | cLangue |
| :------ | :------ |
| 1       | Francais |
| 2       | Anglais |

#### Questions:
+ Q1. Lister les usagers(nom) qui ont des sessions actives;
+ Q2. Lister les sessions qui ne sont pas actives qui ont utilisées le français;
+ Q3. Lister les demandes de rappels de mot de passe qui ont eu lieu le 2019-10-30;
+ Q4. Lister les langues (sans les clés) disponibles en utilisant l'attribut cLangue renommé vers Langage;
+ Q5. Lister les courriels seulement des usagers qui parlent anglais;

----
Auteur :copyright: Guy Francoeur, version A2019

