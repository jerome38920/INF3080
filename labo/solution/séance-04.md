## Solutions Séance-04

### Q1.
  + R' = PROJECTION(cUsager, JOINTURE_NATURELLE(JOINTURE_NATURELLE(Connexion,Session),Usager) )
  
### Q
  + R' = SELECTION(cLanguage='Francais', JOINTURE(Historique,pLangue=pLangue, Langue) )
  + La jointure n'est pas naturelle dans ce cas car il n'y a pas de lien entre les tables (fk)
  
### Q3.
  + R' = SELECTION(dDemande='2019-10-30', Securite)

### Q4.
 + R' = PROJECTION(Langage, ALIAS(cLangue/Langage, Langue) )

### Q5. 
  + R' = POJECTION(cCouriel, SELECTION(pLangue=2, JOINTURE_NATURELLE(Langue, JOINTURE_NATURELLE(Usager,Connexion) )
  
