# MapServer 
![](https://upload.wikimedia.org/wikipedia/commons/f/fe/MapServer.png)

[MapServer](https://mapserver.org/) est l'un des premier serveur cartographique apparu sur le marché (1994). A la base il s'agit d'un projet open source (projet ForNet) porté par [l'université du Minnesota](https://twin-cities.umn.edu/) en collaboration avec la [NASA](https://www.nasa.gov/). Aujourd'hui, MapServer est devenu un projet de [l'OSGeo](https://www.osgeo.org/) et fait parti des serveurs carto les plus performants sur le marché en propose de nombreuses fonctionnalités. Projet totalement open source et développé en C++, il permet de créer des images de cartes géographiques, qui permettent d'orienter les utilisateurs vers du contenu web.

MapServer peut être utilisé principalement de deux manières:
1. Via des APIs appelées MapScript, elles permettent l'utilisation de MapServer directement par une programmation en Python, Java, C et PHP.

2. Utiliser MapServer en mode CGI (Common Gateaway Interface). Cette interface va lancer un programme qui s'exécute par l'intermédiaire d'un serveur Web HTTP, par exemple Apache ou IIS.

La technologie MapServer repose sur un Mapfile qui est l'élément central de l'architecture du serveur cartographique. Il s'agit d'un fichier texte qui définit un certain nombre d'objets garce à un langage balisé propre à MapServer.

## Avantages et inconvénients

**Avantages** : La plus grande force de MapServer c'est sa robustesse. Elles se ressentent dans les performances puisque MapServer et le serveur carto le plus rapide pour la diffusion de données pour les standards OGC.

**Les inconvénients** : MapServer ne possède pas d'interface graphique de configuration. La configuration des couches se fait par l'écritutre de Mapfile dans le cadre d'une utilisation en CGI. Par les APIs MapScript, il faut nécessairement utiliser et donc maîtriser les langages de programmation. 
Dans les deux cas, il faut une phase d'apprentissage avant de pouvoir utiliser MapServer.



## Caractéristiques principales :

- lecture de nombreux formats SIG (Tif, COG, SHP, PostGIS, WMS/WFS)

- export de données dans plusieurs formats SIG (XML, GML, CSV, SHP/ZIP, tuiles vectorielles)

- services et standards de l'OGC : WMS, WFS, WCS, SOS, SLD, OGC API

- stylisation avancée

- catégorisation des classes vectorielles et rasters

- prise en charge des métadonnées Inspire

- support multi-platesformes (Linux, Windows, Mac OS X, Solaris, et plus)

- une multitude de formats de données raster et vecteur (shapefiles ESRI, PostGIS et Oracle Spatial et de nombreux autres formats via GDAL et OGR)

- reprojection de cartes à la volée avec plusieurs milliers de projections grâce à la bibliothèque Proj.4

- très bonnes performances avec très peu d'optimisation requise, ce qui en fait un serveur facile à déployer

- fichiers texte basés pour la configuration, qui peuvent être facilement poussés dans un dépôt git et divisés en plusieurs fichiers de configuration de carte


Standards de [l'Open Geospatial Consortium](https://www.ogc.org/) (OGC) prit en charge dans MapServer :
- Web Map Service (WMS)
- Web Feature Service (WFS)
- Web Coverage Service (WCS)
- Filter Encoding (FE)
- Styled Layer Descriptor (SLD)
- Geography Marhup languge (GML)
- Sensor Observation Service (SOS)