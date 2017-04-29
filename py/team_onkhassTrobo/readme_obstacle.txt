READ ME : d�tection d'obstacles

Les variables robotIP et robotPort sont � pr�ciser

 ############################################

Comment le script s'inscrit-il dans la logique de fonctionnement du robot ?

Avant chaque ordre fourni (au clavier) au robot, il (le robot) doit s'assurer qu'il
n'y a pas d'obstacles � moins de x m�tres de lui. Le robot rend compte de la pr�sence
d'obstacles via des indicateurs :
obstacles_left = 0 : il n'y a pas d'obstacles � gauche
obstacles_left = 1 : il y a un obstacle � gauche
idem pour obstacles_right

Donc :
	- avant chaque ordre lancer la fonction de detection d'obstacle pour actualiser
les variables globales obstacles_left , obstacles_right

	- le groupe travaillant sur les ordres de d�placement doivent prendre en compte
les indicateurs d'obstacles
