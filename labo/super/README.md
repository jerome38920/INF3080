## Super projet de révision

Nous avons dans ce projet toutes les notions vues cette année.

 + Le modèle entité-association a été finalisé pour que vous puissiez compléter. Bravo pour la réflexion.
 + Merci de m'avoir dit que ceratines tables ne sont pas nécessaire.
 + Pas facile de travailler 50 personnes en même temps. :wink:
 + Si des modifications doivent être apporté sur les tables `01_schema.sql` faites le.
 + ajouter dans l'entête de fichier (cp4 date raison)
   - FRAG 2019-11-28 besoin de deux attributs dans la tables employe.
 
### Vous devez compléter 

 + Script de chargement 
   - 50000 lignes dans `machine`;
   - 15000 lignes dans `site`;
   - 7500 lignes dans `detaillant`;
   - combien dans `sitedetaillant` ?
   - 13 provinces et territoires + 1 pays;
   - 100 lignes dans `villes`;
   - 5 lignes dans `modele` + 5 lignes dans `typeMachine`;
   - 50 lignes dans `revision`;
   - 50 lignes dans `employe`;
   - 1000 lignes dans `serviceE`;
   - 5000 lignes dans `serviceD`.
 + Nous avons besoin d'un fichier pour créer les synonymes
 + Nous avons besoin de droits de sélection sur les tables
 + Un script qui enlève les synonymes
 + Un script qui enlève les droits donnés
 + Un script nommé `99_runall.sql` qui appelle tous les scripts 
   
 + **Tout le monde doit contribuer.** 
   - Faites une chose et laissez le suivant continuer;
   - Un fichier par taches;
   - Faire des demandes fusion git;
   - Utiliser de toutes les lignes contenues dans la table lorsqu'il y a des clés étrangères;
   - Le dernier étudiant devra faire l'assemblage de tous les fichiers;
   - Il faut devenir précis dans le nom de vos fichiers afin de créer la bonne séquence d'exécution de script.
 
 + Nous allons continuer avec vos scripts au prochain cours.
   - tentez de rouler tout ... on va voir si ça marche.
 
 ### Nomenclature proposée
 
 Les fichiers aurons les noms suivants :
   + 01_schema.sql
   + 02_sequence.sql
   + 03``lettre``_trigger.sql
      - 03a_trigger.sql :arrow_right: SiteDetaillant
      - b :arrow_right: Detaillant
      - c :arrow_right: ServiceD
      - d :arrow_right: ServiceE
      - e :arrow_right: Employe
      - f :arrow_right: Machine
      - g :arrow_right: Site
      - h :arrow_right: Ville
      - i :arrow_right: Province
      - j :arrow_right: Pays
      - k :arrow_right: TypeMachine
      - l :arrow_right: Revision
      - m :arrow_right: Modele
    + 04`lettre`_charger.sql
    + 05a.sql requêtes 
      - Lister toutes les machines qui ont la dernière révision dans le Québec.
    + 05b.sql
      - à venir
    + 06.sql
      - optimisation
    +
      
 
 ![modele LQ](https://github.com/guyfrancoeur/INF3080/blob/master/labo/super/modele-lq.png)
 
 ## Pourquoi des tables comme ville et province ?
 
 #### Definition - What does Second Normal Form (2NF) mean?
   + Second normal form (2NF) is the second step in normalizing a database. 2NF builds on the first normal form (1NF).
   + Normalization is the process of organizing data in a database so that it meets two basic requirements:
     - There is no redundancy of data (all data is stored in only one place).
     - Data dependencies are logical (all related data items are stored together).
 
 Source : technopedia
 
 ##### FIN.
 ---
 Auteur Guy Francoeur :copyright: 2019
