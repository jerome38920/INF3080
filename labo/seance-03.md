##### Droits d'auteur :copyright: matériel protégé 
 Si vous n'êtes pas étudiant du cours INF3080-030 A2019 vous devez 
 - demander une permission pour l'utilisation de ce matériel;
 - fournir la raison de son usage;

# Séance 3: Modèle relationnel normalisé

- Objectif : Concevoir un modèle relationnel normalisé 
   
----
**Note** : (_facultatif_) S'il y a des questions dans ce labo, répondez y dans un fichier 
nommé `./labo/reponse-labo.md`. Le fichier doit être dans un format `Markdown`. Utilisez 
le projet `inf3080-a2019` pour déposer le fichier `./labo/reponse-labo.md` soit le même
que pour vos exercices.  Utilisez un autre `projet` pour vos travaux pratiques.

##### Format du fichier Markdown
 + Séance 2 (Header 1)
 + Exercice {1..n} (H2)
 + Question {1..n} (H4)
 + S`2`.E`3`.Q`1` (strong) `est une valeur qui change bien sûr`
 + La réponse dans une section script (code block)

**Note**: Il est recommandé de versionner vos réponses aux exercices à l'aide
de Git. Un seul dépôt est amplement suffisant pour tous les laboratoires, en
divisant les fichiers dans des répertoires.

*Conseil* : Vous devriez versionner vos exercices avec Git, afin de
vous entraîner à utiliser le logiciel naturellement.

----

## 1 - Modèle relationnel normalisé

### 1a - module de connexion (gestion des accès) d'une application Web

Vous devez dans cet exercice convertir le modèle conceptuel de la séance précédente en modèle relationnel normalisé. 
Utiliser la notation hongroise telle que vue en classe.

Le module de gestion des accès a les entités suivantes :
 + Usager
 + Connexion
 + Historique
 + Session

Afin d'obtenir un modèle relationnel complet, je vous propose les détails suivants :
 - un usager est associé à une connexion;
 - une session a une date de création;
 - une session a une date d'expiration;
 - l'historique est créé lorsque la session est expirée;

Vous pouvez utiliser [draw.io](draw.io) afin d'accélérer la réalisation.

#### Questions:
+ Q1. Quelle est la difficulté ?
+ Q2. Avez-vous réussi en moins de 35 minutes ?
+ Q3. Produire modèle dans un fichier.

### 1b - module de gestion d'une flotte de camions du style 53'

Maintenant que vous êtes bien échauffé, vous devez maintenant vous mettre dans la tête d'un
informaticien qui a un mandat pour modéliser une partie d'un système pour un transporteur 
majeur (Robert Transport, Guilbeault, Day & Ross).  Vous avez dû les voir sur les routes.

Votre rôle est de faire le modèle conceptuel (déjà fait) maintenant nous ajoutons le modèle
relationnel pour la gestion d'une flotte de remorques + tracteurs (camions).
Vous devez savoir que les camions sont à un seul endroit dans le monde.
La latitude, longitude est utilisé pour situer le camion sur la terre.

En plus de lister des camions, ce que nous voulons maintenir est combien coûte un camion qui roule.
Deux états sont utiles pour le calcul: vide ou chargé (plein).  Vous venez de réaliser qu'une capacité
de chargement est un aspect important de ce domaine.  Vous savez aussi que les camions fonctionnent au
pétrole, diesel (gazoualle) pour certains. Ils n'ont pas tous la même consommation. Les véhicules 
routiers sont identifiables, ont tous une plaque et ont aussi besoin d'une assurance.

Encore, une fois gardez-le tout simple. La notation hongroise est d'usage. Vous pouvez utiliser `draw.io`
pour réaliser le travail.  Dans `draw.io` il y a dans la rubrique `software` un gabarit `database1.xml` 
qui va assurément accélérer la conception. 

Bravo pour vos accomplissements.  Soyez fier.

#### Questions:
 + Q1. Rendre disponible votre modèle en format pdf.

## 2 - Git

Il est important de sauvegarder vos documents dans un gestionnaire de version distant.
Prenez quelques minutes pour créer et pousser vos fichiers.


----
Auteur :copyright: Guy Francoeur
