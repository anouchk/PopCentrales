# PopCentrales
Comment compter la population autour des centrales nucléaires françaises !

L'objectif de ce script est de calculer combien de personnes habitent à proximité des 19 centrales nucléaires françaises. 

En février 2016, le journaliste Philippe Roure avait fait ce calcul sur son blog <a href="http://www.mentrek.org/2016/02/distribution-diode-stable-des-questions.html">Mentrek</a> en utilisant QGIS, ce qui m'a permis de découvrir qu'il existe des données démographiques carroyées de la population européenne.

L'idée est ici de réaliser la démarche de calcul en utilisant Python.

#Etape 1 : combien de Français
J'ai dans un premier temps utilisé le fichier des données carroyées de l'<a href="http://www.insee.fr/fr/themes/detail.asp?reg_id=0&ref_id=donnees-carroyees">Insee</a>. Voir le script popCentrale.py.

#Etape 2 : combien d'Européens 
Réalisant en le faisant que 4 centrales sont à la frontière avec l'Allemagne, le Luxembourg, la Belgique ou la Suisse, j'ai utilisé dans un second temps le fichier des données carroyées d'<a href="http://ec.europa.eu/eurostat/web/gisco/geodata/reference-data/population-distribution-demography">Eurostat</a>. Voir le script popCentrale_euro.py.


#Exploitation journalistique
Ce travail a permis la publication d'une <a href="http://www.aef.info/depeche/libre/532957">dépêche</a> sur le site de l'agence d'informations spécialisée AEF, ainsi qu'une <a href="https://vimeo.com/158511669">vidéo</a> explicative, avec pour outils de datavisualisation une <a href="https://analutzky.cartodb.com/viz/55afc418-e236-11e5-b0ff-0e5db1731f59/public_map">carte</a>, et un <a href="http://datawrapper.dwcdn.net/cW6LD/1/">graphique</a>.

#Suites
Ce travail a été utile par la suite. Le 26 avril 2016, lors de la Conférence Environnementale, Ségolène Royal a <a href="https://twitter.com/RoyalSegolene/status/724919836506202113">annoncé</a> que le périmètre pris en compte en cas d'accident nucléaire grave, pour évacuer et/ou mettre à l'abri les populations passera de 10 à 20 km autour des centrales. Il a été possible d'en mesurer l'impact et de voir que le nombre de personnes concernées passera de de 630 000 à 2,4 millions, soit une multiplication par quatre.
