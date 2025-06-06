# Représentation tangible de la ville

## Contexte
<!-- Initialement la maquette augmentée du LIRIS a été développé par le projet [DatAgora](https://projet.liris.cnrs.fr/vcity/DatAgora/), une collaboration [Erasme](https://www.erasme.org/-DatAgora-333-)/[LIRIS](https://liris.cnrs.fr). 
Le projet de maquette augmentée a continué dans le cadre d'une bourse Marie Curie et sera ensuite amélioré durant la thèse de Corentin Gautier financée par le [LabEx IMU](https://imu.universite-lyon.fr/imu-fr/). -->

Les données urbaines sont de de plus en plus nombreuses et font émerger des outils de médiation complexes sur les villes. Le project Vcity traite et visualise ces données géospatiales pour fournir des représentations de la ville qui permettent de la comprendre. Il offre la possibilité de se promener dans un environnement en 3D et de visualiser les données urbaines sous diverses perspectives. Tout d'abord, ces résultats sont proposés à travers des clients lourds tels que 3DUSE. Cependant, ils empêchent un partage rapide et simple de ces données, ce qui rend les échanges sur les contextes urbains plus difficiles. La méthode UD-SV, notamment UD-Viz, une librairie JavaScript pour visualiser les données spatiales, est plus appropriée pour les clients web.
Sur leur ordinateur, les utilisateurs ont la possibilité de visualiser la géométrie 3D des bâtiments d'un territoire et de naviguer dans cet espace en 3D. Toutefois, il n'est pas nécessairement implicite pour tout le monde de se déplacer dans une scène 3D et il peut être compliqué d'utiliser ces outils de navigation. En outre, même si les instances des clients web sont synchronisées, chacun est isolé derrière son écran, ce qui rend difficile les échanges sur les données urbaines. 
Une première solution pour répondre aux besoins d'un outil de partage urbain est de projeter verticalement les données pour un groupe de participants. La projection permet de rassembler divers profils dans un même endroit, favorisant ainsi l'interaction. La participation a été améliorée en projetant horizontalement (sur une table ou le sol) pour permettre aux participants de se positionner autour de la projection. Cette mesure encourage les participants à interagir davantage avec les données projetées, ce qui enrichit les échanges.    
Les outils de médiation collectifs sont intéressants pour favoriser les échanges entre divers acteurs d'un territoire ayant des niveaux d'expertise différents et pour soutenir les décisions concernant des projets d'urbanisation.

Depuis de nombreuses années, les maquettes utilisées en architecture, en urbanisme ou dans les musées ont démontré leur utilité pour la compréhension d'un territoire. 
Les historiens bénéficient grandement des maquettes historiques car elles permettent de visualiser la structure d'une ville il y a quelques décennies ou des siècles. De plus, ces maquettes peuvent également servir à attirer vers différents sujets urbains, car c'est un outil très expressifs par lui-même.
[Barge](https://archeorient.hypotheses.org/652) décrit les maquettes comme un outil sur lequel s’appuient les échanges scientifiques lors d’un séminaire ou d’une table ronde. Il décrit même la possibilité de manipuler la maquette durant les échanges pour créer des hypothèses d'un territoire. 

Lua et al. compare modèle numérique et modèle physique à travers une enquête quantitative. Ils expliquent que le modèle numérique n'est pas adapté à une certaine tranche d'âge du à leur difficulté de manipuler des scènes 3D numériques. Le modèle physique est plus propice à un outil qui touche un plus large public. La représentation est également plus adapté pour des ateliers participatifs car il ressemble un public dans un même espace.

Buur et Andreasen décrivent la modélisation comme un outil important permettant au concepteur de décrire, de visualiser et de sculpter ses idées lorsqu'il conçoit seul ou lorsqu'il conçoit ou communique avec d'autres.

- Qu'est ce qu'apporte une représentation 3D de la ville
- Parler de l'interet collaborative des maquettes.
    - Papier sur l'interet global d'une maquette (pas forcement urbaine)
    - Livre sur le workshop pour intégrer les citoyens dans les prises de décisions d'urbanistes


TODO : Le contexte peut se voir sous deux facettes :
-	Facette organisationnelle : dans quel cadre institutionnel a été développé Maquette augmentée
-	Facette scientifique et technique : de quoi on part : les limites et ce qu’on recherche : les besoins.
Peut être commencer sur des bases scientifiques : 
    -	Comment faciliter la discussion en matérialisant l’espace ? Utilisation d’une maquette existante ? Utilisation d’une construction (impression 3D, légo)
-	Et voiloù, on arrive sur l’idée de maquette augmentée.
Il me semble que le comment institutionnel est moins important. 
### Projet DatAgora
<!-- Le projet [DataGora](https://projet.liris.cnrs.fr/vcity/DatAgora/) a pour objectif de mobiliser les données et de proposer différentes modalités de visualisation.
Il s'agit d'observer et de mettre en œuvre de nouvelles méthodes de médiation des données, et d'observer cette médiation.
Datagora regroupe des chercheurs de différents dispciplines pour travail autour d'un même dispositif. Ce regroupement permet un croisement des expertises scientifiques et apporte de nouveaux moyens de médiation des données avec des expériences basées initialement sur des travaux de recherche (modélisation, visualisation, médiation, sciences des données, etc.). Il permet la création de nouveaux outils pour aider ces processus de médiations. En rendant ces expériences disponibles dans un lieu physique, ils ont permis de réunir des experts (en mobilité, par exemple) et de les faire échanger sur les scénarios proposés, tout en rendant transparentes les considérations techniques préalables.

Ces dispositifs de médiation sont en analogie avec le fonctionnement des FABLABs. L'objectif est de créer des lieux avec un coût de déploiement assez faible afin de mettre en place un réseau avec des valeurs communes (chartes, méthodes d'utilisation et de production, ouverture à la société, etc.). Ces lieux mobilisent des briques qui peuvent être techniques et scientifiques, qui peuvent ensuite être dupliquées et réutilisées dans de futures expériences. L'approche est modulaire, collaborative et inclusive.
Des salles sont déjà en cours d'expérimentation. Nous pouvons par exemple citer la salle Amigo, la salle Aslan à l'ENS pour le projet DatAgora et une salle à la métropole au sein du laboratoire des Usages Erasme Urban Lab.

Une des principales applications du projet DatAgora a été le projet de végétalisation du quartier Part-dieu. Notre objectif était de proposer un outil de médiation au citoyen afin de cibler les lieux en carence d'espace vert et proposer des scénario de végétalisation.   -->


#### Projet vegetalisation
DatAgora est un projet collaboratif entre l'Université de Lyon et la Métropole de Lyon visant à équiper le territoire métropolitain et ses acteurs d'outils et de ressources pour valoriser et exploiter les données d'intérêt général. Ce projet, créé en 2017 a été financé grâce à un financement de l’IDEX Lyon (de 2017 à 2019) a permis de mettre en place un cadre méthodologique favorisant l’échange entre la recherche et la métropole de Lyon sur l’utilisation des données.


DatAgora adopte des méthodes agiles et se concentre sur l'expérimentation publique, la collaboration, et la médiation des données. Les principaux objectifs de DatAgora incluent :
1.	L'accompagnement de projets liés aux politiques publiques de la Métropole de Lyon
2.	Le développement d'un datalab pour la Métropole, comprenant la conduite de projet, l'apport de ressources techniques, et l'animation de l'écosystème
3.	L'aide à la décision pour la Métropole du Grand Lyon
Un exemple concret de projet réalisé dans le cadre de DatAgora est le calcul d'itinéraires piétons prenant en compte la dimension de fraîcheur, développé en partenariat avec la Métropole de Lyon. DatAgora se positionne ainsi comme un outil innovant pour mutualiser et valoriser les données d'intérêt général, au service des politiques publiques et du développement du territoire métropolitain lyonnais.

<!-- La Part-Dieu est un quartier central dans la vie culturelle et économique de Lyon. C’est un point névralgique du réseau de transports de la ville, ce qui en fait un point d’intérêt crucial à l’échelle européenne. Compte tenu de l’importance de la Part-Dieu pour le développement futur de Lyon et de la France, chaque aspect de ce quartier, chaque changement futur doit être soigneusement étudié et planifié pour assurer sa prospérité. 

Le projet de végétalisation est une collaboration avec “[Le Plan Canopé](https://developpementdurable.grandlyon.com/en-actions/dispositifs-partenariaux/plan-canopee-larbre-au-service-du-climat-urbain/)”, qui vise à planter plus de 300 000 arbres d’ici 2020 dans la métropole lyonnaise. Notre objectif est de montrer les effets de la végétalisation sur la ville pour sensibiliser les élus ou les citoyens à la lutte contre les îlots de chaleur ou la pollution sonore.

Notre problème est de savoir où planter ces arbres pour qu’ils soient les plus efficaces et le moins contraignants possible. Au cours du dernier semestre de 2020, la métropole de Lyon a collecté un maximum de données urbaines qui pourraient être utiles pour traiter et visualiser les parties de la ville les plus adaptées au verdissement de la métropole, même si la première étape est de se concentrer sur la zone de la Part Dieu.

Pour répondre à ce besoin, nous avons développé une maquette 3D de la Part-Dieu, pour interagir avec les données relatives à la revégétalisation de la ville.
La maquette 3D est généré grâce au [legonizer](https://github.com/VCityTeam/Legonizer), un algorithme de transformation de donnée géospatiale en grille de hauteur. Les grilles de hauteurs nous a permis de construire le quartier Part-Dieu en lego. Nous avons construit la maquette en lego car il apporte un aspect ludique à l'outil de médiation et nous permet de moduler plus facilement la représentation. 

En complément de la représentation tangible du quartier, nous projetons des calques des données urbaines à l'aide d'un vidéo projecteur. Ces calques apportent plus de contexte à la maquette et aide à la décision des lieux prioritaires à végétalisés. Ils sont générés sur une base des cadastres de bâtiment de la zone transformé en lego. Cette base est ensuite alimentée par d'autres jeu de donnée 2D urbaines comme par exemple les lignes de transports en communs, les usages des bâtiments etc.. Dans le cadre du projet, les données de plantabilité du quartier nous ont permis de créer un nouveau claque. 

Nous avons collaboré étroitement avec Erasme pour mener à bien ce projet et mettre à disposition cet outil d'aide à la décision pour le grand public et les élus. -->

- [Projet github](https://github.com/VCityTeam/UD-Demo-DatAgora-Vegetalisation-PartDieu)

### Bourse Marie Curie
A la suite du projet DatAgora un nouveau cycle de deux ans sur les maquettes augmentée a débuté. Ce projet a été financé par une bourse Marie Curie obtenu par Arnaud Grignard. L'objectif de ce projet est de développer et déployer le Laboratoire d'Expérimentation Mobile ou maquette augmentée avec l'expérience du MIT qu'a apporté Arnaud Grignard.

Durant ce projet, deux maquettes ont pu être développé avce l'aide des membres du projet VCity (LIRIS). Une maquette version cube (CityScope) qui simulait les personna d'un quartier à l'aide de multi-agents calculé avec l'outil GAMA. Une maquette sur une table de 2m sur 1m qui représentait le quartier Gratte-ciel sur laquelle nous projettions des données urbaines 2D. 
#### Version des maquettes
##### CityScope: 
CityScope est une table démontable / transportable avec une projection sur un territoire en maquette et un écran pour afficher la simualtion. Cet outil a pour objectif le développement d’interface tangible dédiées à la simulation participative en urbanisme.
La projection affiche des multi-agents qui représentent les habitants d'un quartier déambulant en fonction de leur besoin. 
La simulation multi-agents est générée avec [GAMA](https://gama-platform.org) avec l'intégration dans la librairie [UD-Viz](https://github.com/VCityTeam/UD-Viz) pour coupler simulation et visualisation de données 3D géospatiales.
- [Cahier des charges](https://partage.liris.cnrs.fr/index.php/apps/files/?dir=/VCity/Projects/Maquette&openfile=203366209)
- [Projet github ReAgent](https://github.com/VCityTeam/UD_ReAgent_ABM)

##### Maquette de la table:
Le deuxième versions de la maquette développée est une amélioration de ce qui a été mis en place dans le projet DatAgora. Nous sommes partis du même socle logiciel ([legonizer](https://github.com/VCityTeam/Legonizer)) pour générer la maquette physique en lego à partir de donnée open source du Grand Lyon. Ce que nous souhaitions développer est un dispositif transportable avec un support sur lequel poser la représentation tangible et un pied pour placer le vidéo projecteur au dessus. 
Nous avons fait appel à une entreprise pour créer le socle physique et le mât.
- [Table, support maquette](https://partage.liris.cnrs.fr/index.php/apps/files/?dir=/VCity/Projects/Maquette&openfile=203366210)
- 
#### GAMA
Une fois le quartier ciblé et ses données géospatiales traitées, elles ont été intégrées dans une plateforme de modélisation basée sur des agents (GAMA) afin de simuler les actions et les interactions de futurs scénarios urbains potentiels. Cet outil, capable de simuler la dynamique urbaine, a été créé pour aider à la décision des autorités locales et informer le grand public. Il peut être utilisé pour évaluer l'effet de différentes interventions, telles que la piétonisation de certaines zones, l'impact des réseaux électriques distribués ou la répartition des commerces dans une zone dédiée.

Cette phase a également permis d'explorer le couplage de différents types de modèles, principalement des modèles de trafic et de pollution de l'air. Tous les modèles ont été mis en œuvre et mis à jour dans la plateforme GAMA pour la partie ABM et ces simulations ont été par la suite intégré dans les outils [UD-SV](https://github.com/VCityTeam/UD-SV).
Les calques dynamiques de suimulation ont été projeté sur la maquette physique grâce au couplage UD-Viz GAMA. Cet apport nous a permis d'observer que l'outil de médiation est adapté pour de la simulation et peut servir à des experts pour visualiser des données plus complexes. 
<!-- La dernière étape de la phase 1 a été la création de l'interface utilisateur tangible (TUI). Cette interface aide les différentes parties prenantes non expertes à mieux comprendre les processus complexes liés aux différents modèles. Les utilisateurs sont invités à interagir avec le modèle physique et à voir les changements directement sur une carte physique en 3D. -->
#### Les ateliers
##### Ecole de l'Anthropocène : éditions 2022 et 2023
L'objectif était de réfléchir sur le thème du métabolisme urbain avec, comme lieu d'expérimentation, le quartier Gratte-Ciel à Villeurbanne. Lors de cet atelier, des étudiants de l'Université de Lyon ont été réunis à la Maison du projet Gratte-Ciel. Dans cet atelier spécifique, 2 maquettes urbaines ont été déployés afin d'illustrer les dynamiques urbaines dans le quartier:
- Une maquette utilisée pour la visualisation des données représentant une maquette à l'échelle 1/500 du quartier.
- Un module interactif CityScope dédié à l'exploration de la réutilisation des matériaux dans le processus de construction.

##### Atelier bio-inspiré 2022 :
Erasme (Lyon Living Lab) a organisé un sprint d'innovation ouverte sur la thématique d'explorer, questionner et proposer de nouvelles pistes d'usages appliquées à la sphère publique. Il a réuni une soixantaine d'acteurs aux profils variés : chercheurs en biodiversité, modélisation, botanique ou biologie, designers, entrepreneurs et étudiants.
Dans ce cadre, une version spécifique d'un TUI a été développée et déployée. Un jeu interactif de modulation de l'espace public en lien avec les limites planétaires. L'utilisation d'un TUI donne la possibilité de créer des îlots d'usages multiples et interconnectés au sein de la Presqu'île de Lyon pour remplacer les approches rectilignes et unifonctionnelles.

##### Fête de la Science 2022 : 
La version table et la version cube des maquettes ont été déployé et présenté à un public diversifié et large (300 personnes en une journée). Au cours de cette exposition, le projet Gratte-Ciel a été présenté avec les apports du nouveau quartier de 2030 sur la vie à Gratte-Ciel.

### Thèse de CGA

### Le dispositif existant
- [Conception de la maquette physique](../../../Anthropocene_2023/Readme.md) :
- Socle pour la maquette avec projection :
    - [Version cube](./Supports/version-light.md)
    - [Version table](./Supports/version-table.md)

## Problématiques
- **P1:** Comment la maquette augmentée peut devenir un nouvel outil de planification collective ?
    - Développer l'interaction utilisateur.
    - Atelier participatif avec une captation des scénarios d’urbanisation
- **P2:** Lier maquette numérique et maquette tangible, comment manipuler le numérique par le tangible et inversement ? 
    - Capter les changements sur la maquette (manipulation de bâtiment) qui se répercutent sur la réplique numérique.
    - Interaction avec la maquette numérique qui change les calques de projection.
- **P3:** Comment adapter le dispositif en fonction du niveau d’expertise du public ? 
    - Adapter le niveau d’information des calques projetés / de la représentation numérique.
    - Médiateur avec la maquette. Outil qui se suffit seul. 

## Planning 

## Projets de Recherche
- [Page projet](./projet-recherche.md)

## Ateliers - Mise en application
### Passés 
- [Semaine de l'anthropocène](./Anthropocene_2023/Readme.md) (23/01/23 - 27/01/23)
- [Festival pop'science](./Rive-De-Gier_Maquette/Readme.md) (14/05/23)
- [PEPR Ville Durable Bâtiments innovants](./RetoursMaquette.md#pepr-ville-durable-bâtiments-innovants-240523) (24/05/23)
- [GDR IG-RV](./RetoursMaquette.md#gdr-ig-rv-310523) (31/05/23)
- [WPI Project](./StudentProject/WPI_BeyondLego.md) (15/05/23 - 15/06/24)
- [Musée des confluences](./A-quoi-Revent-Les-Maquettes.md) (20/01/24)
- [A quoi rêvent les maquettes ?](./A-quoi-Revent-Les-Maquettes.md#thématique) (22/01/24 - 25/01/24)
### A venir
- [Atelier avec le Rize sur la thématique du logement social](./Ateliers/Rize.md)
- Présentation à la BLM, sujet à définir.
- Mise en application sur la thèse de Aurore Toulou (thèse au CETHIL, Thermique du bâtiment dans notre environnement)


## Bibliographie
* [Tangible table](./../../Bibliographie.md#tangible-table)

## Conférences à viser
- [https://www.reaach.eu](https://www.reaach.eu)
- [https://uist.acm.org/2025/](https://uist.acm.org/2025/) : Deadline - 9 avril (Rank A)
- [https://www.euroxr.org/conference-2025/calls-and-guidelines/scientific-track](https://www.euroxr.org/conference-2025/calls-and-guidelines/scientific-track) : Deadline 13 avril
- [https://www.csis.u-tokyo.ac.jp/3d_geoinfo_sdsc_2025/overview.html](https://www.csis.u-tokyo.ac.jp/3d_geoinfo_sdsc_2025/overview.html) : Deadline - 11 avril

DIS
- User Human interface system
- ACM multimedia system
