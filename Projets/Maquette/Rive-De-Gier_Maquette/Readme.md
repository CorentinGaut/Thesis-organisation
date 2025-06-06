
## Goals
Développement d'une maquette Lego sur le territoire Rive de Gier pour le festival [popSciences](https://popsciences.universite-lyon.fr/) du 13/14 mai 2023.
[IMU](https://imu.universite-lyon.fr/) aura un stand lors de ce festival pour mettre en avant le [projet Rive de Gier](./../TIGA_Vallee-Du-Gier/readme.md). L'intéret, pour les membres du projet, d'ajouter une maquette Lego est d'améliorer leur dispositif de médiation numérique déjà mis en place avec un outil tangible pour aider à la compréhention de ce territoire. En complément l'intérêt pour CGA dans son [projet de thèse](./../Phd_Corentin_Gautier/Readme.md) est d'avoir un nouveau terrain d'expérimentation sur la représentation tangible d'un territoire et d'avoir un retour utilisateur sur cet outil. La maquette Lego sera composé d'une représentation d'une zone industrielle de Rive de Gier, de la table ainsi que son vidéo projecteur pour projeter de la donnée sur la maquette blanche. Le dispositif sera accompagné d'un support de questionnement sur cet outil pour apporter un retour utilisateur sur celui-ci.

La construction de la maquette Lego sera mis en place par CGA à l'aide du widget Legonizer de la librairie [UD-Viz](https://github.com/VCityTeam/UD-Viz#readme).
Les calques de projections seront produits par IMU et projetés grâce au widget SlideShow de [UD-Viz](https://github.com/VCityTeam/UD-Viz#readme). Dans un premier temps la maquette Lego sans projection est la priorité première qui va accompagner le dispositif de médiation proposé par TUBA. Cette médiation sera un scénario/récit que les membres d'IMU devront animer pendant l'atelier.
La projection de donnée sur la maquette pourra être mis en place lors des temps plus calme pendant pop'science mais ne sera pas en même temps que la médiation de TUBA. 

***
## Members :construction_worker:
- **Lead**: [CGA](https://github.com/orgs/VCityTeam/projects/23)
- [CGA](https://github.com/orgs/VCityTeam/projects/23): developer
  * Fournit la maquette légo (réalise l'intégration du légonizer à la démo), 
    le dispositif de projection, intègre les calques de projection,
    réalise le montage/démontage de l'ensemble
  * Présence permanente de deux jours partagée par les membres VCity (GGE doit finaliser parmi LMA, CGA, MLI)
- [LMA](https://github.com/orgs/VCityTeam/projects/8): technical expert
  * Fournit la démo (tout le soft, inclus SlideShow, mais hors légonizer) 
- OPI (Ophélie Pitault, TUBA): secondary product owner
  * Fournit le support de questionnement pour collecter les retours utilisateurs 
- CAU (Clarisse Aubert): lead product owner
  * Présence permanente de 2 jours partagée entre CAU ou CPE 
- CPE (Clémentine Périnaud): secondary product owner
  * Fournit les calques de projection

### Questions ouvertes sur les rôles
* Qui est chargé du transport du matériel sur le site de Festival Pop Sciences ? Il faut demandé à AGR par quelle prestation il est passé pour déplacer la maquette. 
* Finaliser le tableau de présence pour les deux jours du Festival Pop Sciences.
* Est-ce en extérieur ? Si oui, il faut un barnum ! **C'est en interieur**
***

## Effort/Funding
- CGA : 3 jours (hors présence sur site) jusqu'à son départ en Vacances (29/04/23).
***

## Concernant la démo :wrench:
Composants
- UD-Viz/Legonizer Widget
- UD-Viz/SlideShow Widget
- [Démo Rive de Gier](https://github.com/VCityTeam/UD-Demo-IMU-Vallee-Du-Gier-Mockup) entièrement neuve (repository différent de [Vallée du Gier](https://github.com/VCityTeam/UD-Demo-TIGA-Vallee-Du-Gier)) 
  intégrant Legonizer et SlideShow
***
## Requirements/Use-cases/Needs/Design Notes :triangular_ruler:
### Fiche technique Maquette Lego
L'emprise du projet correspond aux bâtiments industriels de SetForge de la vallée du gier. 

<img src="https://user-images.githubusercontent.com/32339907/231222970-696e2e4e-f4ee-4470-bfe5-1f9bb78e07db.PNG"  width="600" height="500">

 - Emprise réel: 320m x 320m 
 - Emprise maquette: 50cm x 50cm = 2 x 2 plaques de Lego

 Echelle de la maquette = 1/640


 Le [Fichier CSV](legoPlates-SetForge-Rive-de-Gier.csv) de construction de la maquette Lego a été généré grâce au Widget Legonizer de UD-Viz. Les paramètres à intégrer dans le widget pour retrouver ce même fichier sont les suivants :
 ```
 Zone selectionnée :
 Position: 1821396, 5144813.869963868, 310.79962664434015
 Rotation: 0, 0, -0.6

 Ratio: 3.5
 Lego plates dimensions: 2, 2
 ```

 Le modèle de lego donnée correspond à l'emprise de setForge définir en amont à la fois sur google map et sur Qgis. Grâce à Qgis nous avons pu récupérer essentiellement les bâtiments de SetForge et sont disponibles en ficheir [.geojson](./BAT_SETFORGE.geojson).
 
 Commande de deux "verres" de Lego plats au magasin lego un de 2x2 et l'autre de 2x4.

***
## To-Do :clipboard:
**Maquette blanche:**
- [X] Définition d'une emprise de la maquette Lego.
- [X] Remise en route du Legonizer.
- [X] Création de la Demo avec le Legonizer et Rive de Gier en data.
- [X] Génération des fiches CSV de la construction de la maquette Lego (Test échelle, observation si les fiches CSV correspondent bien à ce que l'on souhaite).
- [X] Clarifier le nombre de legos manquants et en acheter.
- [X] Construction de la maquette Lego.
- [X] Reconstruction de la table pour déposer la maquette Lego.

**Projection:**
- [ ] Test de la projection sur la maquette Lego (Calibrage/).
- [ ] Création des calques de projections sur la maquette

## Minutes
* [2023 04 11: Discussion sur l'emprise](#fiche-technique-maquette-lego)

***
