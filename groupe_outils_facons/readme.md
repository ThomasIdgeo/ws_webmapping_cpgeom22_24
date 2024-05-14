<p align="center" width="100%">
    <img width="50%" src="https://leafletjs.com/docs/images/logo.png">
</p>
<h2>Définition:</h2>
<p align="center" width="100%">
<img width="10%" src="https://cdn-icons-gif.flaticon.com/6454/6454106.gif">
</p>
<strong>Bibiliothèque Javascript</strong> Open Source édité par Volodymyr Agafonkin dédié à l'affichage de sites cartographiques. De nombreux contributeurs sont également à l'initiative de nouvelles fonctionnalités.
<h2>Historique:</h2>
<p align="center" width="100%">
<img width="10%" src="https://cdn-icons-gif.flaticon.com/7211/7211797.gif">
</p>
Cette bibliothèque a été développé à partir de 2008.
La bibliothèque utilise de format geoJson pour afficher les données depuis 2013.
<h2>Fonctionnalités:</h2>
<p align="center" width="100%">
<img width="10%" src="https://cdn-icons-gif.flaticon.com/6416/6416394.gif">
</p>
Cette bibliothèque supporte les calques 
<li><strong>GeoJson</li> 
<li>Les flux raster WMS/WMTS </strong></li>
ainsi que les données vectorielles 
<li><strong>WFS/PostGis/Shape</strong></li>
De nombreux <strong>plugins</strong> enrichissent également les fonctionnalités de base, comme l'affichage de:
<li><strong>GeoTiff</li>
<li>CSV</li>
<li>Excel</li>
<li>Géocodage</strong></li>
La possibilité de personnaliser les icones et les symbologies des différents types de géométries, tout comme les hachures et les icônes animés peuvent être également insérés.
<h2>Interfaces:</h2>
Des interfaces ont été développées pour permettre l'affichage dans différents langages.
La bibliothèque a été développé en R par la société RStudio, en python la bibliothèque Follium, ce qui permet également de réaliser des cartes.


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

# Geoserveur

![](Logo_Geoserver.png)

## Role

Serveur

## Licence

[GLP](https://www.gnu.org/licenses/gpl-3.0.html)

## Site web

[Site internet](http://geoserver.org/)



## Description

GeoServer est un serveur informatique4 open source et libre écrit en Java qui permet aux utilisateurs de partager et modifier des données géographiques. Conçu pour l'interopérabilité, il publie les données de toutes les sources principales de données spatiales utilisant des normes ouvertes. Source [wikipédia] (https://fr.wikipedia.org/wiki/GeoServer)

## Formats de données acceptés (non exaustif)

- PostGIS
- Oracle Spatial
- ArcSDE
- DB2
- MySQL
- Shapefiles
- GeoTIFF
- GTOPO30
- ECW, MrSID
- JPEG 2000

![](/ressources/mapbox_logo.png)

**Mapbox GL JS** est une librairie Javascript pour la diffusion de cartes sur le web.
## Les formats de données acceptés sont:
- Tuiles vectorielles
- Tuiles raster
- Raster DEM
- GeoJSON

On peut également diffuser des images et des vidéos.
Il est possible de styliser les cartes en utilisant la librairie de style Mapbox GL ou en créant ses propres styles.

  ![](/ressources/openlayer.png)

#### Description 
OpenLayers est une bibliothèque JavaScript permettant d'afficher des données cartographiques dans les navigateurs Web sous forme de cartes glissantes

#### Caracteristiques : fonctionnement

Le principe est simple, pour afficher une carte avec Open Layer, il faut les éléments suivants :

Une page HTML possédant un conteneur (div) qui sera utilisé pour afficher la carte.
Un appel à la librairie Open Layer (pour en utiliser les fonctionnalités).
Un fichier de configuration (pour personnaliser la carte).
Un fichier CSS de mise en forme de la carte.

#### Les fonctionnalités

- Affichage de carte
- Gestion des interactions
- Ajout des données
- Controle de la carte 
- Gestion des couches


#### OpenLayers prend en charge 

- kML 
- GEOJSON 
- WMS
- WSF 
- vecteur
- raster 

####  Utilisation OpenLayers cote serveur :

- Generation des tuiles cartographiques
- Integration avec des services web
- Stockage et gestion des données géographiques

####  Utilisation OpenLayers cote client :

- Intégration dans une page web
- personnalisation de la carte
- gestion des interactions 

# PYGEOAPI  
![](/ressources/pygeoapi_logo.png)

###### PYGEOAPI ([Github](https://github.com/geopython/pygeoapi?source=post_page-----5f52baba731f--------------------------------)) est un serveur Python implémentant le standard OGC API pour la diffusion de données géospatiales.



###### Il est possible de diffuser des données dans plusieurs formats tels que:
>
> - CSV
> - GeoJSON
> - OGR pour les formats SHP ou des flux WFS
> - Des tuiles raster et vectorielles
> - Des données présentes dans une base de données PostgreSQl,MongoDB, Oracle
> - Geopackage
> - ...

###### Il est également possible de permettre des trasactions sur un jeu de données:
> - CREATE, REPLACE, UPDATE, DELETE

###### PYGEOAPI utilise **Jinja** pour rendre des pages HTML et **Flask** pour les réponses HTTP rendues par l'API

###### PYGEOAPI est configurable avec le fichier PYGEOAPI_CONFIG.yml, sur lequel est renseigné:
- les paramètres du serveur
- les ressources utilisées (les sources de données)
- les métadonnées
- les messages logging à afficher en cas d'erreur
