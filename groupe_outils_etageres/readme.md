# Workshop Webmapping 

*Les outils & produits à étagères*

<div align='center'>

# 1 - [LizMap ](https://docs.lizmap.com/current/fr/index.html)

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

### [Architecture LizMap](https://docs.lizmap.com/current/fr/introduction.html)


<hr>

<img src="https://docs.lizmap.com/current/fr/_images/architecture.jpg" >



# 2 - [ArcGis Online !](https://www.arcgis.com/index.html)   
[ArcGis Online](../ressources/arcgis_logo.png)

### Présentation d'ArcGis Online

ArcGIS Online est une solution d’analyse et de cartographie basée sur le cloud. Utilisez-la pour créer des cartes, analyser des données et partager et collaborer. Accédez à des applications propres aux processus, à des cartes et données du monde entier et à des outils qui vous permettent d’être mobile sur le terrain. Vos données et cartes sont stockées dans une infrastructure privée et sécurisée et peuvent être adaptées à vos exigences en matière de cartographie et d’informatique.

<hr>


### Les fonctionnalités d'ArcGis Online

### Créer des cartes

Les cartes interactives créent des expériences immersives qui se détachent des vues statiques et donnent aux utilisateurs la possibilité d’explorer les cartes. La carte s’enrichit de détails et vous apporte de nouvelles perspectives lorsque vous zoomez, effectuez des recherches et interagissez avec les données.

**Importer vos propres données**

Les données existent dans une variété de formats. Avec ArcGIS Online, vous pouvez facilement intégrer du contenu issu du cloud et télécharger des fichiers, y compris des feuilles de calcul, des fichiers au format KML et GeoJSON, ainsi que des fichiers de données géospatiales classiques. Utilisez les outils inclus pour affiner vos données et les préparer à la visualisation et à l’analyse.

**Se connecter à l’IoT et aux données de capteur**

Exploitez des données spatiales en temps réel pour des décisions opérationnelles vitales. Avec ArcGIS Velocity, une fonctionnalité additionnelle, ingérez des données issues de plateformes IoT, de courtiers de messages ou d’API de capteur et appliquez l’analyse en temps réel pour effectuer des actions telles que le geofencing et la détection des incidents.

**Gérer et analyser les données raster et d’imagerie**

Rendez votre imagerie accessible via ArcGIS Online afin que des centaines d’utilisateurs puissent l’exploiter immédiatement. ArcGIS Image for ArcGIS Online est une extension de type d’utilisateur vous permettant d’héberger et d’analyser des données raster et d’imagerie, tout comme vous le faites avec les données vectorielles.

### Partager des cartes et des applications

Partagez des cartes interactives en mode privé avec vos groupes ou publiquement avec tout le monde.

**Choisir qui peut consulter vos cartes**

Choisissez qui peut consulter les cartes que vous créez. Partagez publiquement des cartes qui sensibilisent et incitent à agir. Conservez les cartes confidentielles privées. Vous choisissez qui peut consulter vos cartes à l’aide des paramètres de partage d’ArcGIS Online.

**Intégrer des cartes à votre présence numérique**

Les cartes interactives sont des outils de communication. Elles offrent la possibilité de livrer des récits et partager des informations, tout en incitant les utilisateurs à poser des questions. Vous pouvez partager vos cartes via plusieurs canaux, notamment en les intégrant sur votre site Web, dans les messages publiés sur les réseaux sociaux et dans les articles de blog. Les cartes populaires peuvent être vues simultanément par des milliers de personnes. Vos cartes sont mises à l’échelle et opèrent de manière uniforme sur tous les appareils.

**_Créer rapidement des applications Web interactives_**

Donnez à chacun l’opportunité de s’impliquer facilement avec vos cartes sur n’importe quel appareil en les partageant en tant qu’applications Web interactives. ArcGIS Online inclut des dizaines d’applications que vous pouvez créer en quelques clics. Chaque application remplit un objectif spécifique pour vous aider à livrer votre récit et à maintenir l’intérêt des utilisateurs.

- ArcGis DashBoards :
ArcGIS Dashboards permet aux utilisateurs de communiquer des informations en présentant des analyses géographiques à l’aide de visualisations de données intuitives et interactives sur un seul écran. Toute organisation qui utilise la plateforme ArcGIS peut tirer parti d’ArcGIS Dashboards pour faciliter la prise de décision, visualiser les tendances, surveiller le statut en temps réel et informer ses communautés. Adaptez les tableaux de bord à vos différents publics pour leur permettre de ne garder que les données qui les concernent et obtenir ainsi les réponses dont ils ont besoin. Les tableaux de bord sont des produits d’information essentiels, comme les cartes et les applications, et constituent un élément déterminant pour votre infrastructure géospatiale.

- ArcGis Instant Apps :
ArcGIS Instant Apps appartient à la nouvelle génération d’applications de cartographie Web configurables. Utilisez Instant Apps pour partager vos cartes en tant qu’applications et offrez à votre public une expérience intuitive et orientée qui l’incite à interagir avec les cartes et les données.
Instant Apps inclut une bibliothèque de modèles d’application sans code et une option de configuration rapide lorsque vous voulez personnaliser l’application. Chaque modèle d’application répond un but spécifique, comme afficher une carte ou une scène, comparer des contenus, calculer un itinéraire, explorer une bibliothèque de contenu ou rechercher quelque chose à proximité. Compatible avec les dernières fonctionnalités de Map Viewer, ces modèles sont également optimisés pour les appareils mobiles, prennent en charge plusieurs langues et sont conçus pour utiliser les technologies d’assistance.

- ArcGis Experience Builder :
ArcGIS Experience Builder est une solution hautement configurable dédiée à la création d’applications Web percutantes sans écrire de code. Choisissez un modèle et créez une expérience Web immersive pour votre public en unifiant des cartes Web, des applications, des pages, des widgets interconnectés et des données aussi bien 2D que 3D à travers une interface flexible de type glisser-déposer. Configurez l’apparence de votre application Web sur différentes tailles d’écran et déployez-la dans votre organisation ou pour le public. Concevez des widgets, thèmes et actions personnalisés avec un développement nécessitant peu de code pour étendre davantage votre application Web.

### Collaborer avec des collègues

Travailler efficacement dans l’ensemble de l’organisation en concevant et en utilisant des cartes

**Logiciel de cartographie multi-utilisateur sécurisé**

Collaborez avec vos collègues dans des équipes de toutes tailles dans l’ensemble de votre organisation. Les utilisateurs bénéficient d’un accès simple et sécurisé aux données, cartes et applications dont ils ont besoin pour mener à bien leur travail. Chaque abonnement à ArcGIS Online est géré par son administrateur qui détermine l’accès et les privilèges.

**Travailler en équipe avec des milliers d’utilisateurs**

ArcGIS Online est conçu pour les entreprises, ce qui signifie qu’il répond aux besoins en matière de sécurité, d’authentification, de confidentialité et de gestion des utilisateurs des grandes organisations. Mettez l’intelligence géographique au service de l’ensemble de votre organisation grâce à ce logiciel de cartographie multi-utilisateur sécurisé.

**Collaborer avec des collègues à travers l’entreprise**

Dans une organisation, les personnes occupent de nombreux rôles différents et exécutent une variété de tâches. Certains conçoivent des produits d’information géographique tandis que d’autres les consultent. Les types d’utilisateurs, qui sont les éléments constitutifs des abonnements ArcGIS Online, vous permettent d’attribuer aux membres d’une équipe les fonctionnalités et applications dont ils ont besoin pour mener à bien leur travail.

### Analyser vos données

Appréhendez vos données dans un contexte géographique à l’aide d’outils d’analyse intuitifs. Révélez les relations, identifiez les principales localisations, utilisez les meilleurs itinéraires et analysez les modèles pour établir des prévisions. Apportez un contexte utile à vos données en les associant aux données démographiques et de mode de vie d’Esri.

**Comprendre vos données**

L’analyse est un processus itératif. L’affichage de vos résultats dans une carte interactive permet d’ajuster et d’adapter facilement votre analyse jusqu’à ce que vous obteniez les réponses dont vous avez besoin.
- Analyser les modèles pour formuler des prévisions et déterminer les étapes à suivre
- Identifier les relations et les points aberrants dans vos données
- Associer des données stockées à différents endroits ou ajouter un contexte de localisation à vos données







![Business Geografic](../ressources/bg.png)

# 3 - [GEO Générateur ](https://www.business-geografic.com/fr/geo-software/geo-technologies.html)
Le GEO Générateur de Business Geografic permet de générer rapidement des propres cartes et applications cartographiques HTML5 personnalisées, pour tous publics, sur tous supports, à partir de toutes données géographiques et métier.
Il propose à ses utilisateurs une avance technologique permanente et parfaitement conforme aux recommandations CNIG, OGC et INSPIRE pour la gestion des données et métadonnées.

![GEO Générateur](../ressources/geo.png)

Les données, fonctionnalités, cartes et applications sont des ressources GEO, centralisées au sein d'un catalogue de ressources GEO. Elles sont utilisables dans toutes les applications GEO ainsi que celles des collaborateurs et partenaires avec qui elles sont partagés.

![Menu](../ressources/menu.png)

## Référencez vos données

<b>Connectez-vous</b> directement et simultanément à toutes vos sources de données et métadonnées : bases spatiales, bases métier, web services. Utilisez les intégrateurs et connecteurs métier GEO pour accéder aux données et métadonnées stockées dans vos outils métier. Le GEO Générateur lit nativement tous les standards SIG et formats de données normalisés, en créant des liens dynamiques avec vos données.  

<b>Référencez vos données</b> dans votre Catalogue de Ressources GEO. Scannez vos données, pré-renseignez les champs de vos métadonnées, cataloguez vos données et moissonnez vos métadonnées. Vous pouvez pour cela vous appuyer sur GEO Metadata. GEO respecte, par sa philosophie-même, les recommandations CNIG, INSPIRE et OGC pour la gestion et le partage des données et métadonnées avec vos collaborateurs et partenaires.  

<b>Préparez, classez et organisez</b> vos couches, fonds de plans et thématiques. Créez des champs virtuels. Vous pouvez également créer, gérer, importer et exporter vos couches et thématiques personnelles.

## Créez vos fonctionnalités

<b>Paramétrez sans coder</b> les fonctionnalités que vous souhaitez intégrer dans vos cartes et applications GEO, en exploitant toute la puissance fonctionnelle de GEO. Vos fonctionnalités s’enregistrent dans votre Catalogue de Ressources GEO.  Elles sont transverses à tous vos projets cartographiques. Vous pouvez les partager avec vos collègues et partenaires dans une démarche de mutualisation et de collaboration.
- <b>Recherches et analyses</b> : Définissez vos recherches multi-critères sur toutes vos données spatiales et attributaires. Créez vos analyses simples, par classes et multivaluées ; l’intuitivité offerte par les interfaces utilisateurs GEO offre une approche remarquablement simple pour ventiler, agréger et croiser toutes vos données.
- <b>Fiches d’information</b> : Préparez vos fiches d’information multimédia à partir des modèles GEO ou en créant les vôtres. Utilisez les sections, onglets et pavés déroulants pour structurer efficacement l’information. Vous pouvez lier des fiches d’information entre elles et les enrichir avec tous type de contenus : lien web, flux de données multimédia, etc. 
- <b>Statistiques, tableaux de bord et rapports</b> : Exploitez la puissance de calcul et les nombreux modes de représentation tabulaires, statistiques et cartographiques avancés de GEO. Construisez vos rapports et tableaux de bord par simple cliquer-déposer, pour tous vos besoins de suivi, d’analyse et d’aide à la décision ; paramétrez vos propres modèles d’export selon les mêmes principes ergonomiques.

## Préparez vos cartes

<b>Projetez vos données</b> en cliquant-déposant vos tables, géotables et rasters sur vos fonds de plans.

<b>Paramétrez</b> l’emprise de vos cartes, l’opacité et les seuils de visibilité de vos fonds de plans et couches thématiques.

<b>Editez</b> le style de vos étiquettes et info-bulles ; préparez vos légendes de cartes ; renseignez les métadonnées de vos cartes.

<i>Vos cartes s’enregistrent dans votre catalogue de ressources GEO. Vous pouvez en faire des ressources GEO partagées pour vos collaborateurs et partenaires et les publier sous forme de web services.</i>

## Générez vos applications SIG

<b>Générez et démultipliez</b> en un temps record vos applications cartographiques HTML5 responsive pour tous vos publics, sur tous les supports et à partir de toutes vos ressources GEO : données, fonctionnalités, cartes. GEO favorise la réutilisation et la mutualisation des ressources en permettant, à partir des mêmes ressources GEO, de décliner autant d’applications cartographiques web et mobiles que de besoins professionnels et grand public. 

<b>Choisissez un gabarit de diffusion</b> à usage professionnel ou grand public ainsi qu’un thème graphique ; personnalisez-les en fonction de votre identité visuelle et de vos utilisateurs-cibles.

<b>Générez votre application</b> en cliquant-déposant une carte GEO et en l’enrichissant avec les fonctionnalités et modules fonctionnels GEO de votre choix. Votre application se génère sous vos yeux en mode HTML5 responsive natif ; elle s’adapte automatiquement aux écrans des tablettes et smartphones pour vous affranchir des développements mobiles spécifiques. 

<b>Publiez vos applications cartographiques</b> en un clic, via des liens web personnalisables ou au sein de vos supports web existants (portails Extranet, outils Intranet, sites Internet, etc.). Vous pouvez également les diffuser sous forme d’applications mobiles dédiées et les référencer dans les « mobile app stores ». Vous pouvez en outre les partager sous forme de web services ou utiliser les API GEO pour les exploiter directement dans vos progiciels métier. 

Vos applications cartographiques GEO sont générées une seule fois pour tous les supports : ordinateurs, tablettes, smartphones.

Elles sont facilement démultipliables et personnalisables en fonction de vos publics, de leurs besoins et attentes spécifiques :
- <b>applications professionnelles</b> : intégrez vos cartes GEO dans les gabarits de diffusion à usages professionnels ; vos collaborateurs et partenaires pourront ainsi exploiter l’ensemble des fonctionnalités et outils métier GEO, en modes web et/ou mobile, connecté et/ou déconnecté. 
- <b>applications grand public</b> : intégrez vos cartes GEO dans les gabarits de diffusion à usage grand public et/ou déclinez vos applications grand public à partir de vos applications métier GEO existantes ; vos cibles grand public apprécieront la modernité et la richesse de vos applications, qu’ils les utilisent en modes web et/ou mobile, connecté et/ou déconnecté. 

A l’instar des données, fonctionnalités et cartes GEO, vous pouvez partager vos applications cartographiques GEO avec vos collègues, homologues et partenaires, pour mutualiser vos ressources et développer l’entraide. GEO assure une gestion fine des droits de vos utilisateurs et groupes d’utilisateurs sur vos ressources GEO partagées.




# 4 - [Mviewer](https://fr.pornhub.com/)

## Présentation de solutions 

mviewer est un Visualiseur géographique basé sur OpenLayers 6.3.1 et Bootstrap 3.3.6.

mviewer est une application cartographique initiée et développée par la 
Région Bretagne, sous le nom de Kartenn (carte en breton). Le code source de cette application est librement réutilisable depuis 2014.

## La communauté 
Mviewer une application open-source co-construite par des acteurs de compétences et d’origines diverses.

## Fonctionnalite 
Visualisation carto, chiffre clés (des tableaux , des garphique, des fichers), data visualisation (photo, textes, vidéo)


## les avantages 

Simple, rapide, modulaire, ergonomique publier l'applications avec des données géographiques, des graphiques et du contenu éditorial pour les diffuser sur vos sites institutionnels et sur tous les supports.

## Installation
Mviewer est une application web développée en HTML / CSS / JAVASCRIPT. Elle nécessite simplement d’être déployée sur un serveur WEB qui peut être APACHE, NGINX, TOMCAT


# 5 - SOGEFI
<img src="https://www.sogefigroup.com/static/upload/sog/sogefi-group.gif" />


# 6 - VMAP
<img src="https://sig.agglopole.fr/images/vmap.png">


vMap2 est une application web qui permet de représenter, gérer et éditer les données localisées (géospatiales) des entreprises et organisations de manière compatible avec leur système d’information. 

Elle est exploitée dans de nombreux secteurs d’activité :  

Travaux publics pour visualiser l’état des réseaux d’éclairage public et gérer les interventions, 
Collectivités locales pour fournir des informations sur la propriété foncière aux citoyens,  
Producteurs d’énergie pour prioriser les zones de production photovoltaïques 
Transport pour gérer des voies cyclables au niveau national 
Producteurs de données pour commercialiser une offre de service 

vMap2 s’appuie sur une pile logicielle complète fournissant des solutions pour le stockage, l’édition et le calcul en mode on-premise ou bien dans le cloud AWS : PostgreSQL, PostGIS, MapServer, Angular, PHP… 

Grâce à la plateforme d’intégration de données FME (Safe Software), vMap2 s’interface naturellement avec votre Système d’Information d’entreprise et peut exploiter toutes les sources de données de votre organisation : Oracle, MySQL, SQLServer, Excel, Text, XML… 

### Que faire avec vMap2 ?


Publiez sous forme de carte l’emplacement de votre patrimoine, de vos clients, de vos prospects…
Editez vos données en créant des formulaires de saisie personnalisés 
Exploitez des sources de données libres (OSM, IGN…) comme fond de carte 
Recherchez une adresse, un lieu-dit, une commune 
Développez et commercialisez un service pour votre métier 

### Sécurisé par conception

La sécurité est à la base de la conception de vMap2.

La fiabilité de l’application est régulièrement soumise à des tests d’intrusion par des structures indépendantes. 