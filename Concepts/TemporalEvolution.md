# Concept of temporal evolution data
**Mots clefs**
- Chronotope / Temporal / Visualisation

**Questionnements:**
- Comment visualiser un graphe de scénario de la donnée ?
- Comment montrer l'évolution morphologique de ces données 3D dans une scène géospatiale ?
- Comment représenter le temps dans une visualisation 3D ?

- Scénario , incertitude ? 

**Utilisateurs:**
- Les chercheurs pour visualiser leur graphe de donnée de scénario possible de celle-ci.
- Les historiens pour comparer les évolutions de morphologie urbaine sur un quartier.
- Les citoyens pour comprendre leur quartier.

## Mature
## Immature
### Morphologie des bâtiments Texture:
Montrer l'évolution de la donnée 3D à l'aide de motif de texture pour montrer un changement d'etat. Par example une destruction pourrait être simuler par une texture sur le bâtiment avec plusieurs flèches pointant vers le bas oualors inversement pour montrer une construction. Il faudrait que cette texture se créée entre 2 millésimes de donnée et faire une petite animation pour montrer l'évolution et le rendre plus dynamique.

 ![image](https://user-images.githubusercontent.com/32339907/205876549-e9789f07-eb31-4ad6-b184-3a40722d495a.png)
 
 Comment créer la texture pour ensuite l'appliquer à un bâtiments du jeu de donnée et voir pour l'animer ?
- Référence :
 - [Visualization of Data Changes in 2.5D Treemaps usingProcedural Textures and Animated Transitions](https://dl.acm.org/doi/10.1145/3481549.3481570)
 - Pour faire une texture animer = [lien](https://pierfrancesco-soffritti.medium.com/animations-with-alpha-textures-in-three-js-52a33654e137)

### Barre temporelle :
L'objectif est de montrer les données disponibles sur le slider temporel afin de faire un premier tri des données pour l'utilisateur. De manière intuitive l'élément html montrera la ou il y a beaucoup d'évolution de donnée ou alors la ou on a le plus d'information. Il faut que l'utilisateur puisse en un seul coup d'oeil capter la ou il y a le plus d'informations à visualiser et montrer les époques ou il y a eu le plus de changements.

  ![image](https://user-images.githubusercontent.com/32339907/205881744-0189bff1-d093-41aa-b653-4cc137fd9cfb.png)
  
  Il faudrait chercher les données dans le layer manager, générer dynamiquement les "dots" qui représenteront les layers sur le slider temporel avec un jeu de couleur pour différencier les types de données. Par example, on pourrait imaginer que les données 3D des bâtiments pourrait être en vert ou alors on differencie le type des bâtiments (résidentiels / industrie / commerce) Le slider sera à doubles entrée, on pourra afficher / cacher les données qui seront dans le champs du doubles sliders afin d'être plus précis dans la visualisation.
  - Référence : [4D browser](https://4dbrowser.urbanhistory4d.org/explore/51.049329,13.738144?map=1911&from=1820-01-01&to=2012-12-06&undated=1&model=1930-01-01)



### Slider temporel sur la vue
Comme à la "Remonté le temps" de l'IGN, comparer la géométrie à l'aide d'un slider qui change l'espace d'une des deux vues qui ont une temporalité différentes. Il faudra que ca soit à l'échelle du quartier (je pense) car sinon on ne verra pas beaucoup les modification.
 
https://remonterletemps.ign.fr/   adapté à la 3D. 

Ou alors faire avec 3D vue qui rajoute la vue de transition de change detection 

![image](https://user-images.githubusercontent.com/32339907/205946587-e759666d-341d-4d54-a805-8cf272c23061.png)

### Communication entre donnée de flux et donnée géometrique

Il faudrait réflechir comment lié une donnée de flux, comme le flux de travailleur entre leur lieu de travail et leur lieu de résidence peut être assimiler avec les données géometriques et notamment donner une explication sur l'évolution du quartier et les flux qui évoluent.

Il faut peut être dissocier les deux modes de rendu 

### Travail avec l'intégration du modèle de donnée de DVA
Intégration de différents scénario possible de la donnée, avec un graphe pour voir ce qui est plus facilement intégrable et permettre une interaction.
**Possible axes de développements:**
-  **Le times cube geometry** : Plutôt que de superposer les données pour montrer les changements morphologiques, il faudrait créer des couches de layers qui se mettent les une au dessus des autres avec un petit décalage pour bien visualiser les couches. La couches la plus hautes serait la couches la plus récentes et plus on descend plus les données sont anciennes. Sur chaque couche on mettrait une étiquette qui serait la date de la donnée et on pourrait faire un lien (avec une ligne) entre les couches sur chaque bâtiments qui aura eu un changement d'etat entre millésimes. L'axe du temps serait représenté par l'axe z de la scène 3D. Cela reprend le principe du space time cube sauf que le temps évolue dans l'autre sens, il faudrait tester de faire dans l'axe inverse et voir si l'utilisateur comprends bien l'évolution. Pour chaque évolution rajouter une couleur qui donnera le type de changement entre les millésimes. En plus de ça il faudra montrer ces changements sur les bâtiments et mettre une opacité différentes sur les bâtiments non selectionnée. 

![image](https://user-images.githubusercontent.com/32339907/205889637-c3da4b5e-b838-4e20-a031-c4e4f47198df.png)


- Le slideur temporel mettrait en avant les scénarios des bâtiments sur une fourchette de temps. Entre les deux balises seulement la donnée de ces millésimes seront affichés dans la scène afin de pouvoir choisir les couches que l'on souhaite comparer. 
- La selection en graphe des bâtiments pourrait permettre de se focaliser sur un seule bâtiments et voir son évolution. il mettrait en avant le bâtiments et changerait l'opacité des autres pour les mettres en retrait. Un lien avec une ligne en couleur entre chaque millésimes permettrait de mieux se rendre compte de la liaison. En fonction de la couleur cela permettrait de donner une indication du type de changement de la morphologie du bâtiment avec une légende comme un texte à côté du lien.
- Change detection permettrai de donner l'indication des changements d'etat et devrait être plus facilement avec id du Geometry layer. 


