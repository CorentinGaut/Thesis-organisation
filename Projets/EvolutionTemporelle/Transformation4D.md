# Méthodes de transformation des levels
**A CLEAN**
## Space-Time cube
### Représentation


- Un scale de plus en plus petit plus on monte dans le STC. Pour ne pas cacher les layers d'en dessous.
### Time Scale
Chronological, l'espacement entre les versions de la donnée est proportionnel à la chronologie. Un coefficient calculé avec la boudning box de la verion est ajouté pour mettre de l'espace entre les levels et ne pas avoir un effet de supperposition. 
Le temps peut être dans les deux directions possibles. 
## Elipse
### Représentation


**Matrice de transformation**:

Le rayon du cercle autour de la zone doit être plus grand que la bounding box que la version à analyser afin que le cercle ne soit pas trop petit au dessus de la version centrale et ne pas perdre en lisibilité. 
Le cercle des versions est placé plus en hauteur pour plusieurs raisons. Le terrain de la zone à analyser peut être irrégulier et être uen zone montagneuse et donc le sol cacherai les autres versions de la ville. L'autre raison est que si on met à plats ces versions il y aurait uen confusion avec la position géospatiales des nouvelles versions et donc on détache les versions du cercle pour ne pas faire le lien avec le sol. 

**2 modes de représentations:**
* Le mode global: la version au centre du cercle est la level le plus ancien. Les autres versions autour de la zone à analyser ont une opacité de 1 et un scale plus petit de 0.5. Les versions du cercle se positionnent toujours de la même manière en fonction de la camera. La version la plus ancienne sera celle qui serala plus proche de la camera. 

* Le mode analyse d'une version: L'utilisateur sélectionne une version dans l'arc de cercle. Le level sélectionné se place au centre du cercle. Les versions $i-1$ et $i+1$ ont un scale de 0.8 et une opacité de 1. Les autres versions ont une opacité de 0.5 et un scale de 0.5 pour mettre en avant la version à analyser. Les différences de géometrie s'affichent entre la version au centre et les versions $i-1$ et $i+1$. 


### Time Scale
Sequential: En fonction du nombre de version disponible, celles-ci se placent de manière equidistantes le long du cercle de représentation. Cette représentation est plus adapté pour peu de version de la ville car au bout d'un certain nombre les versions se supperposent et la représentation devient illisible.  

## Spirale
### Représentation
### Time Scale
Chronological:


## Vecteur
### Représentation

**Matrice de transformation**

La translation en z reste la même que le space-time cube initial avec l'espace en temps et le height des levels. Un décalage en "arrière" est effectué en fonction du point de vue de la caméra. Ce décalage supplémentaire permet d'avoir plus de visibilité sur tout un quartier en évolution, la ou seulement la disposition en z peut empécher de voir certaines évolutions dans l'axe spatio-temporel.

La version la plus ancienne est celle qui est à plat sur le fond de carte. Les autres levels sont disposés dans l'espace et avec une legère rotation x et y vers la camera et fait toujours face à la camera en orientation z. Cette rotation permet d'avoir une vision de tout les levels dans n'importe quel point de vue.

**Transactions**

Les types de changements peuvent être difficile à suivre le long de l'axe temporel. Un lien symbolique entre les versions nous permet de suivre plus facilement l'évolution d'un bâtiment et observer les différents changements opérer pendant durant une époque. 

### Time Scale
Chronological: Les versions suivent la suite logique temporel des versions. Avec un espace entre les versions en fonction de la boundings  box des levels pour eviter l'effet de supperposition en cas de gratte-ciel dans la donnée.
 