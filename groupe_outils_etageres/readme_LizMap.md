# Workshop Webmapping 

*Les outils & produits à étagères*

<div align='center'>

## 1 - LizMap 

<img src="https://docs.lizmap.com/current/fr/_static/logo.png">

 Important : La version de Lizmap Web Client requiert

*Firefox ≥ 63* ; *Edge ≥ 79* ; *Chromium ≥ 54* </div>
<hr>



LizMap est une application web cartographique <b>*OpenSource* </b> développée par la société 3Liz qui fonctionne soit sur Apache soit sur Nginx. C'est une application écrite en PHP.

Elle utilise QGIS Serveur pour diffuser ses données en lien WMS/WMTS.

L'application LizMap reflète le projet QGIS conçu. C'est à dire, que lorsque le projet est bien paramétré, nous retrouvons exactement la même cartographie que dans QGIS. 
Pour une optimisation de l'utilisation de LizMap, il faut que la version de QGIS soit la même que la version de QGIS Server. Par exemple, si l'on utilise la version 3.28 de QGIS, QGIS Serveur doit être en 3.28. 

L'installation de LizMap est disponible en ligne de commande ou via docker. 

La légende affichée dans le navigateur web respecte l'ordre et l'organisation définie dans QGIS. 
<hr>

### Configuration des cartes dans QGIS

<hr>
Lors de la création d'un projet QGIS que nous voulons diffuser dans LizMap, la configuration dans QGIS permet de faire :

- Ordre et structure de la légende

- Symbologie des couches

- Carte de situation grâce à la présence d’un groupe Overview

- Configuration des templates d’impression via les composeurs

*Attention, le projet QGIS doit être enregistré au format qgs et non qgz comme par défaut*

<hr>

### Plugin LizMap

<hr>

Le plugin LizMap est téléchargeable dans les **extensions de QGIS**. Lors de son installation et après avoir bien installé le LizMap web client disponible sur Github, il suffit de paramétrer l'adresse IP et on peut commencer à configurer le projet pour qu'il soit disponible en ligne. Dans le plugin LizMap, il est possible de :

- préciser le nom des couches et des groupes dans l’interface Web

- regrouper les couches en une seule couche WMS

- définir certaines couches comme couche de fond

- définir le système d’affichage : image seule ou ensemble de tuile

- définir la durée de vie de l’image dans le cache

- définir la durée de vie d’une image sur le réseau

- définir les popups d’interrogation des couches

- définir un lien vers la fiche de métadonnées

- définir les échelles de consultation de la carte

- définir les outils accessibles avec la carte :

- impressions

- mesures de longueurs, surfaces et périmètres

- utilisation de la géolocalisation de l’utilisateur (GPS)

- recherche d’adresse dans OpenStreetMap, Google ou Géoportail IGN

- Définir les fonds de plan externe :

- - Google Maps

- - Bing Maps

- - OpenStreetMap

- - Géoportail IGN

- Définir les couches servant de raccourci de navigation :

- - recherche dans le champ d’une couche

- - zoom sur l’élément sélectionné

- - recherche en cascade au sein de la même couche via 2 attributs ou entre couches jointes

<hr>

### Autres possibilités

<hr>

Dans LizMap, il est possible d'ajouter ses propres actions. L'ajout de cette fonctionnalité permet d'aller interroger directement en ajoutant un fichier .actions dans la structure de l'installation du code. Cela permet d'aller interroger la base de données PostgreSQL et de faire apparaître les géométries sélectionnées. Par exemple, on peut sélectionner un certain nombre de bâtiments qui sont à 1 kilomètre à vol d'oiseau d'un bureau de poste. 

Pour des actions plus avancées, il est possible d'ajouter son propre JavaScript qui en fonction des identifiants des couches QGIS, permet d'interroger celles ci. 

On peut aussi faire des filtres en fonction de l'utilisateur qui se connecte. Par exemple si, un utilisateur veut voir uniquement les données de sa commune plutôt que toutes les données de son département, il pourra les apercevoir avec un filtre spatial conçu récemment. 

<hr>

### Architecture LizMap


<hr>

<img src="https://docs.lizmap.com/current/fr/_images/architecture.jpg" >