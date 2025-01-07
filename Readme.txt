
Le projet "Trouver des films similaires à partir des résumés" utilise des techniques de traitement du langage naturel (NLP) 
et de regroupement pour analyser les similitudes entre les résumés de films. Voici une explication concise de l'approche :

Jeux de données : 
   Utiliser deux datasets contenant les titres des films et leurs résumés provenant d'IMDb et de Wikipedia.

Prétraitement du texte :

  Combiner les résumés des deux sources.
  Effectuer la tokenisation pour diviser le texte en unités (mots ou phrases).
  Appliquer la racisation (stemming) pour réduire les mots à leur forme racine.

Vectorisation :

  Convertir le texte en données numériques à l'aide de TF-IDF (Fréquence Terme-Fréquence Inverse de Document), une méthode qui met en valeur les mots importants.
  Regroupement :

  Utiliser l'algorithme KMeans pour regrouper les films ayant des résumés similaires.
  Calculer les scores de similarité (par exemple, en utilisant la similarité cosinus) pour évaluer les relations entre les clusters.

Visualisation :

  Utiliser des outils comme Matplotlib pour créer des dendrogrammes et représenter visuellement les relations hiérarchiques entre les clusters.