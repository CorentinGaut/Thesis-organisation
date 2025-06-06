# Veille sur les données de simulation

Voir [projet de recherche](./projet-recherche.md).

## Formats de données

### 3D Tiles

Standard pour la visualisation web de données géospatiales massives (nuages de points ou meshes). Les données sont réparties en tuiles hiérarchisées et "streamées".

Liens :

- [3D Tiles Specification](https://github.com/CesiumGS/3d-tiles)
- [OGC](https://www.ogc.org/standard/3dtiles/)
- [Datasets Liris](https://dataset-dl.liris.cnrs.fr/three-d-tiles-lyon-metropolis/)

### OBJ

### VTK (format)

Question : comment créer du .vtk ?

### CityGML

### STL

## Librairies

### VTK

Librairie C++, nécessite une compilation avec CMake

Version 9.3.0

Liens :

- [Téléchargement](https://vtk.org/download/)

## Outils

### Py3DTilers

Liens :

- [Py3DTilers](https://github.com/VCityTeam/py3dtilers)
  - [CityTiler](https://github.com/VCityTeam/py3dtilers/tree/master/py3dtilers/CityTiler#city-tiler) : CityGML vers 3DTiles via une base 3DCityDB
  - [ObjTiler](https://github.com/VCityTeam/py3dtilers/tree/master/py3dtilers/ObjTiler#obj-tiler) : OBJ vers 3DTiles
- [Exemples de 3DTiles créés avec Py3DTilers](https://py3dtilers.vcityliris.cma.alpha.grandlyon.com/)

### 3D Tiles Generation using VTK

Liens :

- [Article Kitware](https://www.kitware.com/3d-tiles-generation-using-vtk/)
- [Tiler](https://github.com/Kitware/Danesfield/blob/master/tools/tiler.py)

Le tiler.py permet de transformer de la donnée (CityGML, vtp, las, laz, obj) vers du 3D Tiles

- Semble nécessiter de build VTK en local

En utilisant `pip install vtk`, la plupart des modules VTK sont présents mais il manque `vtkIOGDAL`, ce qui empêche l'execution de `tiler.py`.

#### Installation on Windows

Download and install Visual Studio Community and C++ tools

Add the path to the compiler to the `Path` environment variable. The path should look like this: `C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Tools\MSVC\14.29.30133\bin\Hostx64\x64`

Download and install [CMake](https://cmake.org/download/)

Download [Ninja](https://github.com/ninja-build/ninja/releases). Add the path to the __folder__ containing `ninja.exe` in `Path` environment variable.

In a terminal, run:

```bash
mkdir -p vtk
git clone --recursive https://gitlab.kitware.com/vtk/vtk.git vtk/source
cd vtk
cmake -G Ninja -DVTK_WHEEL_BUILD=ON -DVTK_WRAP_PYTHON=ON source
```

### VTK Js

Installation avec Node et npm :

```bash
npm install @kitware/vtk.js
```

Dans un `package.json` :

```json
  "dependencies": {
    "@kitware/vtk.js": "^30.10.0",
  },
```

Permet de visualiser du .vtk, du .vtp, de l'OBJ, du STL, du Draco

Une demo VTK Js + Node est disponible [ici](https://github.com/LorenzoMarnat/VTK_JS-Demo)

### ParaView

Version 5.13.0

Liens :

- [Téléchargement](https://www.paraview.org/download/)

Supporte les formats : CityGML, OBJ, STL, VTK, PLY, etc

Exporte notamment dans les formats OBJ, PLY, STL, VTM (VTK multi blocks avec fichiers vtp) (pas CityGML ni VTK)

Notes :

- Pour charger le CityGML de Data Grand Lyon, il faut séléctionner le LOD 2 (Properties --> LOD --> 2 --> Apply)
- Beaucoup de difficultés à charger des gros fichiers CityGML
  - Plante avec le BATI 2018 CityGML (fonctionne avec de petits fichiers, comme Tour Part Dieu)
  - Fonctionne avec le TIN (pourtant parfois bien plus lourd que le bati)
- CityGML -> STL : fonctionne bien avec le terrain (TIN) mais pas avec le bati (trop de surfaces, 1 fichier par surface)

### UD-Viz

Visualisation de données géospatiales, basé sur [iTowns](https://github.com/iTowns/itowns)

Version 4.2.0

Liens :

- [Téléchargement](https://github.com/VCityTeam/UD-Viz)

## Diagrammes

![format drawio](https://github.com/VCityTeam/VCity/assets/32875283/b9630570-f918-43a5-afbe-f5a91a2c1f60)
