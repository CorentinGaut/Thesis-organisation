# Concept of hybrid models
## mature
## immature
### Level of abstraction
Il faudrait essayer lors de la construction de la maquette Lego changer le niveau de détails de certains quartier ou des zones que l'on veut mettre plus en avant. Par example por Gratte-Ciel, mettre les bâtiments de 1930 plus détaillés et les alentours construire de simple block blanc pour se focaliser sur les bâtiments essentiels et mettre plus en avant ceux qui nous interesse. Pour ça soit il faudrait le produire dans le code une zone spécifique pour plus de détails ou alors le faire à la main et documenté. 

### Legonizer in UD-Viz
Reprendre tout le concept du Legonizer qui est fait dans Unity pour l'intégrer dans UD-Viz avec le même principe de selection qu'utilise IMU pour reproduire la mini maquette. Au dela de reprendre tout ce code il faudrait l'améliorer en rajoutant des paramètres pour qu'on puisse plus facilement comprendre l'échelle de la maquette.
Le code devra selectionner une zone et en fonction des paramètres voulu (nombre de plaques lego, longueur, largeur...) produira les grille csv pour construire la maquette ainsi que le nombre total de lego. En plus des grilles CSV il faudrait une prés visualisation de ce que ça peut donner en lego. Il faudrait l'afficher dans UD-Viz directement pour pouvoir faire ses testes au même endroit. 

### Kinect Interaction
Placer une kinect au dessus de la maquette qui reconnait tout les bâtiments. Chaque bâtiment pour être déplacé afin de créer une ville modulable, la kinect reproduira sur un ecran à côté de la maquette tangible son jumeau numérique et se mettra à jour en fonction des modification qu'on apportera sur celle en physique. L'objectif et de rajouter plus d'interaction avec le dispositif de médiation et créer des scénarios d'une nouvelle ville pour des architectes ou urbanistes. 
