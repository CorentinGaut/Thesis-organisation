# Comité de suivi de thèse 

Information sur le CST [ED info/math](http://edinfomaths.universite-lyon.fr/these/suivi-de-these)
Date CST : 14/05/2024


## Introduction
Ma thèse a débuté en octobre 2022, dans le cadre du projet TIGA une des actions de l’appel à projet de l’Etat du programme « Territoires d’Innovation ». L’action est pilotée par l’Université de Lyon en particulier par le Labex IMU et porte sur le prototypage, l’expérimentation et la valorisation de méthode et d’outils pour la médiation industrielle. Dans ce contexte, mon sujet de thèse a pour objectif de développer de nouvelles modalités de représentation du territoire à la fois tangible, numérique et dynamique.  La thèse est co-encadrée par Gilles Gesquière (Origami) et Johanna Delanoy (Origami).

## Résumé des travaux effectués
Les jumeaux numériques des villes se font de plus en plus nombreux pour décrire facilement un territoire. Nous voulons améliorer ces dispositifs de médiation en ajoutant plus d’information qu’une représentation 3D des bâtiments. 

###	Intégration de multimédia dans un modèle urbain 3D numérique
Une première idée pour améliorer les jumeaux numériques est l’intégration de contenu multimédia tel que des documents, vidéos, images d’archives ou interview. Ces supports sont une autre manière de décrire une ville et combiner les deux modes de représentation permet de contextualiser le modèle 3D de bâtiment. Grâce à un état de l’art, nous avons remarqué que les approches proposées n’intégraient pas forcement tout type de multimédia ou n’était pas adapté pour un modèle 3D de ville. Nous avons proposé quatre méthodes d’intégration de contenu multimédias dans une scène 3D géospatiale. Ces méthodes nous permettent de gérer les contenus vidéos/images/interviews/document tout en le liant aux données urbaines géospatiales et ainsi décrire une ville sous différent format. Ces travaux de recherche ont été publié à la conférence internationale 3DGeoInfo & SDSC 2022 [1] et ont été présentés à Sydney le 20 novembre 2022. 

###	Représentation de l’évolution de la ville
Ensuite, nous nous sommes intéressés à la représentation l’évolution de la donnée 3D pour mieux comprendre comment a évolué une ville. Plusieurs approches représentent la ville à instant t, notamment les travaux de Jaillot. Toutefois, elles ne montrent pas l’ensemble de l’évolution dans une même représentation avec une vision globale des changements. 
Nous avons proposé une première approche afin de visualiser l’ensemble de l’évolution de la ville. Notre première méthode reprend la représentation du space-time cube, utilisé pour visualiser des données temporelles tel que des flux, en l’adaptant aux données 3D du territoire. L’idée du space-time cube est que le temps est représenté par l’axe verticale z. Nous superposons les versions de la ville dans cet espace 4D (3D + temporel) afin de comparer changements morphologiques des bâtiments. Entre chaque niveau, nous intégrons des liens de couleur qui relient la géométrie d’un bâtiment au cours du temps. Ces liens sont colorés en fonction de l’état de transaction de la donnée (Destruction en rouge, Modification en jaune et Construction en vert). Gautier al. [3].
En complément de ces travaux, nous nous sommes orientés sur d’autres manières d’intégrer les versions dans un espace 3D. Le space-time cube utilisant l’axe z pour disposer les versions, nous voulons proposer 3 approches supplémentaires (cf. Figure 1) qui s’emparent de tout l’espace 3D pour faciliter la compréhension de l’évolution. Ces approches sont définies sous forme de timeline et donne une direction aux versions à placer dans l’espace. Le long de ces timeline nous proposons également 3 manières de positionner les versions pour visualiser différemment les évolutions.


###	Modélisation tangible d’un territoire
La représentation numérique nous permet d’avoir un outil de perception de la ville plus accessible avec son support web. Toutefois, les maquettes physiques sont des outils qui ont fait leur preuve dans des musées pour la médiation autour d’une thématique. Nous nous sommes inspirés des maquettes tangibles du MIT pour produire une maquette d’un quartier de Lyon à l’aide des données 3D géospatiales des bâtiments. Nous avons développé un algorithme permettant de prendre de la donnée 3D géospatiale en entrée pour la transformer en carte des hauteurs des Legos à placer. Nous utilisons du Lego blanc afin d’augmenter la maquette en projetant des données 2D urbaines. La projection permet d’ajouter plus d’information à un territoire et offre une nouvelle dimension à la maquette. Pour impliquer l’utilisateur de manière plus active, nous souhaitons apporter plus d’interactivité au dispositif. L’objectif est que la maquette puisse être manipulé pour créer des scénarios d’urbanisation d’un territoire.  Pour cela, nous voulons capter les changements qu’a apportés un utilisateur comme des déplacements de bâtiments, ou de lego de couleurs qui simuleront un autre objet urbain. Avec ces changements la projection se met à jour et permet d’avoir un retour direct de ce que l’action effectuée à comme répercussion sur la ville. 


## Perspectives pour la deuxième année
   L’intégration de multimédia dans un modèle 3D numérique de la ville permet une annotation des bâtiments ou d’un quartier. Les prochains travaux sont de combiner la représentation évolutive de la ville avec ces contenus multimédia pour donner plus de contexte à des changements dans la ville. Par exemple placer les schémas d’architecte qui justifie la destruction de certain bâtiment à la couche de donnée correspondant à la date de destruction. Pour la maquette Lego, nous voulons un expérimenter des représentations de la ville sous différents niveaux d’échelles en fonction du discours qu’on souhaite raconter autour de cet outil de médiation.
## Valorisation / Formations scientifiques
### Publications


- 3D GeoInfo / SDSC : [Integrating multimedia document in 3D city model for a better understanding of territories](https://hal.science/hal-03852790/) (19-21/10/2022)
- Mappemonde : [UD-SV : Plateforme d’exploration de données urbaines à n-dimensions — Espace, Temps, Thématiques](https://journals.openedition.org/mappemonde/8265) (11/04/2023)

<span style="color:green"> 
<ul>
    <li>IV23: <a href = "https://hal.science/hal-04200467/document">Representation of urban geometry evolution through space-time cube</a> (27/07/23)</li>
    <li>Computer Graphics Forum: Evolutive 3D Urban Data Representation through Timeline Design Space (En cours)</li>
</ul>
</span>


### Séminaires/Réunions
- (*Présentation*) [Challenge GeoDatadays 2022:](https://www.geodatadays.fr/page/GeoDataDays-2022-Les-Challenges-Geodata/113) UD-SV (14/09/2022) **Premier prix du Jury**
- (*Présentation*) [MAGIS-AP3D:](https://github.com/VCityTeam/MAGIS-AP3D/blob/master/Media/README.md) Intégration de multimédia dans une maquette 3D de la ville pour une meilleur compréhension des territoires (06/04/2023)
- (*Participation*) [Origami](https://projet.liris.cnrs.fr/origami/index.html) - Mondes Virtuels: groupe de lecture autour de la génération procédurale de terrains (Toutes les 3 semaines)
- (*Participation*) [Journée d'étude : La boite à outils de cartographie et de la géovisualisation de données](https://github.com/magisAR9/JEGeovizRennes) (06/01/2023)
- (*Participation*) Journée des doctorants ED Info/Math Lyon: présentation des sujets de thèse des D2. (23/02/2023)

<span style="color:green"> 
<ul>
    <li>(<i>Participation / Organisation </i>) <a href="https://imu.universite-lyon.fr/journees-imu-2024-inscriptions-ouvertes-/"> Journées IMU </a> - Intelligences des mondes urbains. Organisation des journées (accueil des invités, participations aux ateliers etc..). Participation à la table ronde des doctorants - Les thèses pluridisciplinaires au labEx IMU (4-5/04/2024)</li>
 </ul>
</span>

### Ateliers
- [Semaine de l'anthropocène "A quoi rêvent les maquettes ?"](https://ecoleanthropocene.universite-lyon.fr/a-quoi-revent-les-maquettes--289281.kjsp?RH=2023prog): Développement d'une maquette augmentée du quartier Gratte-ciel,  mise à disposition pour des étudiants pluridisciplinaires ([Page projet](../../Anthropocene_2023/Readme.md)). (23-27/01/2023)
- [Festival pop'sciences 2023](https://popsciences.universite-lyon.fr/le_festival/) : Développement d'une maquette hybride de la vallée du Gier ([Page projet](../../Rive-De-Gier_Maquette/Readme.md)). (12-14/05/2023)

<span style="color:green"> 
<ul>
    <li><a href="https://www.univ-gustave-eiffel.fr/luniversite/nos-projets-transformants/programme-et-equipement-prioritaire-de-recherche-pepr">PEPR Ville Durable Bâtiments innovants</a>: Inauguration du PEPR Ville durable Bâtiments innovant à Paris. Présentation du dispositif de maquette augmentée mobile avec comme maquette lego le quartier Gratte-Ciel (24/05/2023)</li>
    <li><a href="https://gdr-igrv.fr/">GDR IG-RV:</a> Regroupement de chercheurs dans le domaine de l'informatique géométrique et graphique, la réalité virtuelle et la visualisation. Présentation du dispositif de maquette augmentée mobile avec le quartier Gratte-Ciel(31/05/2023)</li>
    <li><a href="https://www.museedesconfluences.fr/fr/agenda/la-science-de-leau">Musée des confluences - La science de l'eau:</a> Collaboration avec un étudiant de l'école universitaire H2O'Lyon sur une projection de son projet de fin d'etude sur la table augmentée. (20/01/2024)</li>
    <li><a href="./../Projets/Maquette/RetoursMaquette.md#retours-maquette-tangible">"A quoi rêvent les maquettes ?":</a> Atelier de médiation sur le Learning center du campus de Bron. Projection de donnée sur la maquette existante du bâtiment. Suivi des différents groupes d'étudiants dans l'atelier. Mise en place du dispositif de maquette augmentée. (22-25/01/2024)</li>
</ul>
</span>

### Formations doctorales
<span style="color:green"> 
<ul>
    <li>T-TH4-1 / Gestion des conflits et des personnalités difficiles (12-27/10/2023) (12/10/2023 - 27/10/2023) - 14 heures</li>
    <li>T-COM1-2 / Préparation au concours Ma thèse en 180 secondes (édition 2024) (27/11/2023 - 16/01/2024) - 12 heures</li>
    <li>T-COM5-1 / Créer un dispositif de médiation scientifique (sept-oct 2023) (18/09/2023 - 7/10/2023) - 30 heures</li>
 </ul>
</span>

Total : 56h

## Encadrement/Enseignement
- GAMAGORA DU Infographiste: initiation à la programmation. Le programme est du scripting Blender, des cours de Scratch et de la programmation d'un jeu vidéo dans Unity. (40h)
- Beyond Lego WPI: encadrement d'étudiants du Worcester Polytechnic institute. Leur objectif est de produire un état de l'art des maquettes lego existantes et d'avoir un esprit critique sur les dispositifs trouvés.
