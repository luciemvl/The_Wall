# The_Wall  
IF36 project  
  
  
## Introduction  

### Données  

Voici le dataset que nous avons choisi : https://www.kaggle.com/datasets/uciml/student-alcohol-consumption  
  
Ces données ont pour origine une recherche sur des étudiants dans deux écoles secondaires au Portugal en 2008. Il s'agit d'**une grande variété d'attributs des étudiants, y compris des informations sur leur situation sociale, sur leurs études, etc.** Ces données sont à l'origine utilisées pour effectuer une prédiction des notes des étudiants avec l'exploration de données. Elles sont aussi utiles pour rechercher la relation entre ces attributs des étudiants et ainsi inspirer des améliorations sur la pédagogie.   
  
Le dataset consiste en 2 documents csv et 1 document R. Le document student-mat.csv représente des informations sur des étudiants dans le cours de math et le document student-por.csv sur ceux dans le cours de Portugais. À l'aide du document student-merge.R on peut accéder aux informations des étudiants qui apparaissent dans tous les deux groupes.   
  
Nous avons choisi ces données pour des raisons suivantes :   
+ Nous disposons avec ce dataset d'une grande quantité de variables qui nous donne de nombreux sujets d'études possibles.   
  
Une description des données :   
+ 396 étudiants sont étudiés dans le groupe du cours de math et 650 étudiants dans le groupe du cours de Portugais. 382 étudiants apparaissent dans les deux groupes.   
+ Dans chaque groupes, 33 attributs sont étudiés.   
> school - student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira)
> sex - student's sex (binary: 'F' - female or 'M' - male)
> age - student's age (numeric: from 15 to 22)
> address - student's home address type (binary: 'U' - urban or 'R' - rural)
> famsize - family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)
> Pstatus - parent's cohabitation status (binary: 'T' - living together or 'A' - apart)
> Medu - mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 – 5th to 9th grade, 3 – secondary education or 4 – higher education)
> Fedu - father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 – 5th to 9th grade, 3 – secondary education or 4 – higher education)
> Mjob - mother's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
> Fjob - father's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
> reason - reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other')
> guardian - student's guardian (nominal: 'mother', 'father' or 'other')
> traveltime - home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)
> studytime - weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)
> failures - number of past class failures (numeric: n if 1<=n<3, else 4)
> schoolsup - extra educational support (binary: yes or no)
> famsup - family educational support (binary: yes or no)
> paid - extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)
> activities - extra-curricular activities (binary: yes or no)
> nursery - attended nursery school (binary: yes or no)
> higher - wants to take higher education (binary: yes or no)
> internet - Internet access at home (binary: yes or no)
> romantic - with a romantic relationship (binary: yes or no)
> famrel - quality of family relationships (numeric: from 1 - very bad to 5 - excellent)
> freetime - free time after school (numeric: from 1 - very low to 5 - very high)
> goout - going out with friends (numeric: from 1 - very low to 5 - very high)
> Dalc - workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
> Walc - weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)
> health - current health status (numeric: from 1 - very bad to 5 - very good)
> absences - number of school absences (numeric: from 0 to 93)

### Plan d'analyse  

Nous nous avons posé des questions suivantes :   
+ Existe-t-il une relation entre

  
***
Je ne suis pas sûr que j'ai bien compris tout ce qui est demandé...   
S'il y a des choses dont on a pas besoin tu supprimes...et si tu trouves des erreurs de grammaires ou d'autres choses tu peux corriger :)  
Merci !   
