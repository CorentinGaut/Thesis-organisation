## Maillage dual
Un maillage dual est une construction géométrique qui permet de créer un nouveau maillage à partir d'un maillage existant. Voici les principales caractéristiques et utilisations du maillage dual :
### Définition et construction
Le maillage dual est obtenu en suivant ces règles :
- À chaque face du maillage original correspond un sommet dans le maillage dual.
- À chaque arête du maillage original correspond une arête dans le maillage dual.
- Deux sommets du maillage dual sont reliés par une arête si et seulement si les faces correspondantes dans le maillage original partagent une arête commune.

### Propriétés importantes
1. Bijection des arêtes : Il existe une correspondance biunivoque entre les arêtes du maillage original et celles du maillage dual.
2. Nombre d'arêtes conservé : Le nombre d'arêtes reste identique entre le maillage original et son dual, ce qui s'exprime par |E(G)| = |E(G*)|, où G est le graphe original et G* son dual.
3. Application aux graphes planaires : Le concept de maillage dual est particulièrement pertinent pour les graphes planaires, c'est-à-dire les graphes pouvant être dessinés dans le plan sans que leurs arêtes ne se croisent.

### Applications et exemples
1. Diagramme de Voronoï et triangulation de Delaunay : Le dual d'une triangulation de Delaunay est le diagramme de Voronoï correspondant.
2. Analyse de structures : En géométrie computationnelle et en analyse de maillages, le dual permet d'étudier les relations entre les éléments du maillage sous un angle différent.
3. Optimisation de maillages : La dualité peut être utilisée dans certains algorithmes d'optimisation de maillages, permettant de passer d'une représentation à l'autre pour améliorer certaines propriétés.

### Remarques importantes
- Le maillage dual n'est défini que pour un graphe planaire plongé dans le plan.
- Le maillage original et son dual peuvent être des multigraphes, c'est-à-dire qu'ils peuvent contenir des arêtes parallèles et des boucles.
En résumé, le maillage dual offre une perspective alternative sur la structure d'un maillage, permettant d'analyser et de manipuler les données géométriques d'une manière complémentaire à l'approche originale.

## Formule d'euler
### Applications pratiques
Cette formule permet de :
- Déterminer l'existence de solutions pour des problèmes de parcours optimaux, comme le problème des ponts de Königsberg.
- Optimiser des itinéraires dans des réseaux de transport ou de distribution, en identifiant les circuits qui passent par toutes les connexions une seule fois.
- Analyser la structure de réseaux dans divers domaines comme l'informatique, la logistique ou les télécommunications.
### Caractérisation des graphes eulériens
Le théorème d'Euler établit que :
- Un graphe connexe admet un cycle eulérien (un circuit qui passe une et une seule fois par toutes les arêtes et revient au point de départ) si et seulement si tous ses sommets sont de degré pair.
- Un graphe connexe admet un parcours eulérien (un chemin qui passe une et une seule fois par toutes les arêtes sans nécessairement revenir au point de départ) si et seulement si tous ses sommets sont de degré pair, sauf éventuellement deux d'entre eux.
### Algorithmes et résolution de problèmes
Le théorème d'Euler sert de base à des algorithmes pour :
- Trouver un cycle ou un parcours eulérien dans un graphe, lorsqu'il existe.
- Vérifier rapidement si un graphe est eulérien, en examinant simplement les degrés de ses sommets.

## Projection Oblique
La projection oblique est une technique de représentation graphique utilisée pour créer des images bidimensionnelles d'objets tridimensionnels.

### Définition et principes
C'est un type de projection parallèle où les rayons projetants intersectent le plan de projection à un angle oblique.
Elle permet de représenter un objet sur un plan en suggérant un effet de profondeur.
Une face du solide est représentée dans le plan principal en vraies grandeurs, tandis que les autres faces sont projetées obliquement.

### Propriétés
Le parallélisme des segments de la figure est conservé.
L'une des faces de l'objet est parallèle au plan et projetée sans déformation.
Les projections des deux autres faces fuient vers la droite ou la gauche.
Les sphères sont projetées comme des ellipses sur le plan de dessin, contrairement à la projection orthogonale où elles apparaissent comme des cercles