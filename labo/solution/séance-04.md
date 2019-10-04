## Solutions Séance-04

### Q1.
  + R' = PROJECTION(cUsager, JOINTURE_NATURELLE(JOINTURE_NATURELLE(Connexion,Session),Usager))
  
### Q2.
  + R' = SELECTION( JOINTURE(Historique,pLangue=pLangue, Langue), cLanguage='Francais')
  
### Q3.
  +

### Q4.
 + R' = PROJECTION (Langage, ALIAS(cLangue/Langage, Langue) )

### Q5. 
  + R' = POJECTION(cCouriel, SELECTION(pLangue=2, JOINTURE_NATURELLE(Langue, JOINTURE_NATURELLE(Usager,Connexion) )
  
