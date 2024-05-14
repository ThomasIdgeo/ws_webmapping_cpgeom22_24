# PYGEOAPI  

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
