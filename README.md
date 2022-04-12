
# The_Wall  
IF36 project  
  
  
## Introduction  

### Données  

Voici le dataset que nous avons choisi : https://www.kaggle.com/datasets/uciml/student-alcohol-consumption  
  
Ces données ont pour origine une recherche sur des étudiants dans deux écoles secondaires au Portugal en 2008. Il s'agit d'**une grande variété d'attributs des étudiants, y compris des informations sur leur situation sociale, sur leurs études, etc.** Ces données sont à l'origine analysés pour effectuer une prédiction des notes des étudiants aux examens finaux. Elles sont aussi utiles pour rechercher la relation entre ces attributs des étudiants et ainsi inspirer des améliorations sur la pédagogie.   
  
Le dataset consiste en 2 documents csv et 1 document R. Le document student-mat.csv représente des informations sur des étudiants dans le cours de math et le document student-por.csv sur ceux dans le cours de Portugais. À l'aide du document student-merge.R on peut accéder aux informations des étudiants qui apparaissent dans les deux groupes.   
  
Nous avons choisi ces données pour les raisons suivantes :   
+ Nous disposons avec ce dataset d'une grande quantité de variables qui nous donne de nombreux sujets d'étude possibles.   
+ Un sujet touchant à l'éducation nous intéressant tout les trois.
+ Nous étions curieux de voir quelle influence pouvait avoir la consomation d'alcool sur les résultats scolaires
+ La variété des attributs est assez forte.
+ Les attributs étudiés sont explicites. Il ne s'agit pas de données trop techniques : nous allons pouvoir rentrer dans le détails de l'analyse sans nous soucier de la complexité des variables étudiées.
  
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

Dans un premier temps, il s'agirait de faire une étude globale de nos données. Cela nous permetterait de définir un contexte à notre travail d'analyse. Par exemple même si l'intervalle entre les individus les plus jeunes et les plus âgés n'est pas grand, voir si l'âge est un élément déterminant. Même chose pour le sexe et les autres attributs qu'on pourrait qualifier d'élémentaires (la liste de ceux-ci restera à définir). Il pourrait se réveler intéréssant de voir si nous pouvons déjà tirer quelques tendances en mettant en relations ces éléments et les comportements vis-à-vis de l'alcool.  
Dans un second temps nous rentrerons dans le détail, y-a-t-il une corrélation entre résultats scolaire et consommation d'alcool directe. En effet, nous pouvons supposer facilement qu'il y a un lien important entre ces deux élements. Seulement, nous pensons que les choses ne sont pas si simples. Il serait trop rapide de conclure sur le fait qu'un seul facteur est la cause de l'échec scolaire. 
+ CONJECTURE:  
Les élements cités ci-dessus nous amènent à penser que l'échec scolaire est influencé par la consommation d'alcool de manière chaînée. En effet, la consommation d'alcool peut provoquer des aléas qui conduisent potentiellement à l'échec scolaire. Seulement, ces aléas se créent dans un contexte ou un milieu propice à leur apparition. Il est donc nécessaire d'étudier l'écosystème de vie global d'un étudiant afin de voir si l'impact de l'alcool est significatif. Nous voulons arriver à montrer la complexité du problème afin de le traiter dans son ensemble.
+ RESULTATS ESCOMPTES:  
Nous pensons réussir à montrer facilement que le phénomène auquel nous nous intéressons est cyclique. Si un étudiant a une trop forte consommation d'alcool, il y a de forte chance que l'étude de certains attributs montre qu'il évolue dans environnement qui l'influence négativement, et donc que ces résultats soient moins bons. A l'inverse, s'il est avéré que l'étudiant se trouve dans un environnement peu propices de part différents aspects, cela peut être propice à une consommation d'alcool trop élevée et donc à des résultats médiocres.  
Dans cette optique, nous comptons définir ce que voudrait dire "consommation trop élevé". Est ce que les étudiants qui consommerait en semaine seraient plus impactés ? Est ce que la quantité consommée est un facteur important ?  
Il nous faudra également définir ce qu'est un éco-système propice ou peu propice. La profession des parents joue-t-elle un rôle? Le climat familial ? La santé ?  
La variable rendant compte du nombre d'absence va nous etre trés utile car elle pourra trés certainement etre un indicateur révélateur pouvant faire le lien pour ce qui a été expliqué précédement (éco-systeme mauvais => alcool => absence => mauvais résultat).  

Études possibles sur les variables  
> Exemple 1  
> > Sujet : Relation entre la consommation d'alcool en semaine et le nombre d'absence   
> > But : Essayer de trouver comment la consommation d'alcool affecte la vie étudiante    
> > Méthode possible : Point graph, coloré avec le sexe  
> > Problème potentiel : les données se concentrent dans une partie de l'échelle, ce qui peut rendre difficile l'établissement de la relation.   
>   
> Exemple 2  
> > Sujet : Relation entre l'âge des étudiants et leur temps libre   
> > But : Essayer d'obtenir une partie de l'image de l'évolution de l'écosystème des étudiants au cours du temps, ce qui peut être en relation avec le stress, le choix de divertissements, etc. et au final, être relié à la consommation d'alcool à l'aide d'autres études
> > Méthode possible : (Traitement en avance pour obtenir le temps libre moyen) Line graph  
> > Problème potentiel :  l'échelle 1 à 5 de la variable temps libre peut être trop subjective.   
>   
> Exemple 3  
> > Sujet : Relation entre l'éducation des parents et le nombre de ratés  
> > But : Essayer de trouver l'impact de l'environnement familial sur les résultats de l'étudiant (il reste à vérifier avec d'autres études comment ce facteur intéragit avec la consommation d'alcool et influencer les résultats de l'étudiant)  
> > Méthode possible : Point graph  
> > Problème Potentiel : on est toujours au risque de ne pas trouver une corrélation signifiante.   
***  
> Exemple  
> > Sujet : Raison du choix de l'école  
> > Méthode Possible :  Histogram  
> > Problème potentiel :  Les raisons sont peu variées
