# The_Wall  
IF36 project  
  
  
## Introduction  

### Données  

Voici le dataset que nous avons choisi : https://www.kaggle.com/datasets/uciml/student-alcohol-consumption  
  
Ces données ont pour origine une recherche sur des étudiants dans deux écoles secondaires au Portugal en 2008. Il s'agit d'**une grande variété d'attributs des étudiants, y compris des informations sur leur situation sociale, sur leurs études, etc.** Ces données sont à l'origine utilisées pour effectuer une prédiction des notes des étudiants avec l'exploration de données. Elles sont aussi utiles pour rechercher la relation entre ces attributs des étudiants et ainsi inspirer des améliorations sur la pédagogie.   
  
Le dataset consiste en 2 documents csv et 1 document R. Le document student-mat.csv représente des informations sur des étudiants dans le cours de math et le document student-por.csv sur ceux dans le cours de Portugais. À l'aide du document student-merge.R on peut accéder aux informations des étudiants qui apparaissent dans tous les deux groupes.   
  
Nous avons choisi ces données pour des raisons suivantes :   
+ Nous disposons avec ce dataset d'une grande quantité de variables qui nous donne de nombreux sujets d'étude possibles.   
  
Une description des données :    
+ 396 étudiants sont étudiés dans le groupe du cours de math et 650 étudiants dans le groupe du cours de Portugais. 382 étudiants apparaissent dans les deux groupes.   
+ Dans chaque groupes, 33 attributs sont étudiés.   
> school - école de l’étudiant (binaire: 'GP' - Gabriel Pereira ou 'MS' - Mousinho da Silveira)  
> sex - sexe de l’étudiant (binaire: 'F' - féminin ou 'M' - masculin)  
> age - âge de l’étudiant (numérique: 15 à 22)  
> address - type d’addresse domicile de l’étudiant (binaire: 'U' - urbain ou 'R' - rural)  
> famsize - taille de la famille (binaire: 'LE3' - inférieure ou égale à 3 ou 'GT3' - supérieure à 3)  
> Pstatus - état de cohabitation des parents (binaire: 'T' - (together) ensemble ou 'A' - (apart) séparé)  
> Medu - éducation de la mère (numérique: 0 - none, 1 - primary education (4th grade), 2 - 5th à 9th grade, 3 - secondary education ou 4 - higher education)  
> Fedu - éducation du père (numérique: 0 - none, 1 - primary education (4th grade), 2 - 5th à 9th grade, 3 - secondary education ou 4 - higher education)  
> Mjob - travail de la mère (nominal: 'teacher', 'health' relatif à la santé, 'services' civils (administratif, policier, etc.), 'at_home' ou 'other')  
> Fjob - travail du père (nominal: 'teacher', 'health' relatif à la santé, 'services' civils (administratif, policier, etc.), 'at_home' ou 'other')  
> reason - raison du choix de l’école (nominal: 'home' près du domicile, 'reputation' (école), 'course' préférence des cours ou 'other')  
> guardian - gardien de l’étudiant (nominal: 'mother', 'father' ou 'other')  
> traveltime - temps entre le doimcile et l’école (numérique: 1 - <15 min., 2 - 15 à 30 min., 3 - 30 min. à 1 hour, ou 4 - >1 hour)  
> studytime - temps de travail par semaine (numérique: 1 - <2 heures, 2 - 2 à 5 heures, 3 - 5 à 10 heures, ou 4 - >10 heures)  
> failures - nombre de ratés (numérique: n si 1<=n<3, sinon 4)  
> schoolsup – support éducatif supplémentaire (binaire: yes ou no)  
> famsup – support éducatif familial (binaire: yes ou no)  
> paid – cours supplémentaires payés sur les sujets du cours (Math ou Portugais) (binaire: yes ou no)  
> activities – activités périscolaires (binaire: yes ou no)  
> nursery – être allé à l’école maternelle (binaire: yes ou no)  
> higher – volonté de l’éducation supérieur (binaire: yes ou no)  
> internet – accès à l’internet au domicile (binaire: yes ou no)  
> romantic – avoir une realtion romantique (binaire: yes ou no)  
> famrel – quatlité des relations familliales (numérique: 1 - très mauvaises à 5 - excellentes)  
> freetime – temps libre après les cours (numérique: 1 – très bas à 5 – très haut)  
> goout – sortir avec des amis (numérique: 1 – très bas à 5 – très haut)  
> Dalc – comsommation d’alcool en semaine (numérique: 1 – très bas à 5 – très haut)  
> Walc - comsommation d’alcool en weekend (numérique: 1 – très bas à 5 – très haut)  
> health – état de santé actuel (numérique: 1 – très mauvais à 5 – très bon)  
> absences – nombre d’absences (numérique: 0 à 93)  

### Plan d'analyse  

Dans nos études sur ces données, nous allons : 
+ Comparer des variables
> Nous pouvons trouver la relation entre des paires de variables (parfois prenant en compte d'autres). 
> 
> > Exemple : Relation entre la consommation d'alcool en semaine et le nombre d'absence. 
> > 
+ Analyser des variables seules
> Nous pouvons étudier la répartition dans les étudiants d'une variable (parfois prenant en compte d'autres). 
> Nous pouvons
> > Exemple : Raison du choix de l'école
> > 

  
***
Je ne suis pas sûr que j'ai bien compris tout ce qui est demandé...   
S'il y a des choses dont on a pas besoin tu supprimes...et si tu trouves des erreurs de grammaires ou d'autres choses tu peux corriger :)  
Merci !   
