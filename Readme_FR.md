# XboxToolsSuite V2 - Français

XboxToolsSuite V2 est une suite d'outils pour travailler avec les fichiers de ressources, textures et meshes de la première Xbox.

## Fonctionnalités

### Application principale

- Organisation en onglets :
  - XIP Tools
  - XBX Tools
  - XMTools
  - Options
- Aperçu mesh avec OpenGL moderne
- Splash screen transparent
- Choix du logo du splash screen
- Mode splash non transparent avec contour
- Redémarrage de l'application depuis le menu File

### XIP Tools

XIP Tools sert à inspecter, modifier, créer et extraire les archives Xbox XIP.

Fonctionnalités :

- Ouvrir une ou plusieurs archives `.xip`
- Créer une nouvelle archive XIP
- Sauvegarder l'archive courante
- Sauvegarder toutes les archives modifiées
- Glisser-déposer des fichiers `.xip`
- Ajouter des fichiers dans une archive
- Remplacer des fichiers existants avec confirmation
- Supprimer les entrées sélectionnées
- Renommer une entrée
- Extraire la sélection
- Extraire toute l'archive
- Rechercher/filtrer dans l'archive
- Afficher ou masquer les internal buffers
- Gestion multi-onglets
- Menu clic droit sur les onglets :
  - Save As
  - Close
  - Close Others
  - Close All
- Icônes Xbox personnalisées pour :
  - XIP
  - XBX texture
  - XM mesh
  - XAP
  - Audio
  - Fichiers génériques
- Prévisualisation XBX directement depuis une archive XIP
- Prévisualisation XM depuis une archive XIP via l'onglet XMTools

### XBX Tools

XBX Tools convertit les textures Xbox et les images classiques.

Modes de conversion :

- IMG -> XBX
- XBX -> PNG
- ALL

IMG -> XBX :

- Formats d'entrée supportés :
  - PNG
  - JPG
  - JPEG
  - BMP
- Sortie XBX/XPR native en DXT3
- Mode qualité Fast
- Mode qualité High
- Vérification des tailles power-of-two
- Vérification des contraintes DXT par blocs

XBX -> PNG :

- Formats d'entrée supportés :
  - `.xbx`
  - `.xpr`
- Formats texture supportés :
  - DXT1
  - DXT2 / DXT3
  - DXT4 / DXT5
  - A8R8G8B8
  - X8R8G8B8
- Décodage ARGB swizzled
- Sortie PNG

Outils :

- Convert
- Clear Log
- Open Input Folder
- Open Output Folder
- Nettoyage optionnel du dossier de sortie avant conversion
- Console de log/progression
- Dossiers par défaut créés automatiquement :
  - `img2xbx_IMG`
  - `img2xbx_XBX`
  - `xbx2png_XBX`
  - `xbx2png_PNG`

### XMTools

XMTools gère les fichiers mesh Xbox `.xm`, DirectX `.x` et Wavefront `.obj`.

Formats supportés :

- Xbox Mesh `.xm`
- DirectX Mesh `.x`
- Wavefront OBJ `.obj`

Fonctionnalités Mesh Tools :

- Ouvrir `.xm`, `.x`, `.obj`
- Prévisualiser les meshes avec OpenGL moderne
- Modes d'affichage :
  - Total View
  - Solid Shaded Optimized
  - Realistic Shaded
  - Wireframe
- Convertir `.x` vers `.xm`
- Convertir `.xm` vers `.x`
- Convertir `.obj` vers `.xm` ou `.x`
- Conversion batch :
  - `.x` -> `.xm`
  - `.xm` -> `.x`
- Exporter le mesh courant en OBJ
- Ouvrir un OBJ dans l'onglet intégré OBJ Editor
- Arbre d'information mesh :
  - Source du fichier
  - Polygons
  - Vertices
  - Indices
  - FVF
  - Stride
  - Bounding box
  - Taille du mesh
  - Centre
  - Bounding sphere
  - Vertex format
  - Vertex buffer layout
  - Index buffer
  - Statistiques mesh
  - Coordonnées de texture
  - Analyse des faces
- Menu contextuel mesh :
  - Set Mesh FVF
  - Center Mesh
  - Reset Transform
  - Scale x0.5
  - Scale x2
- Déplacement clavier dans Mesh Tools :
  - Flèches : déplacer sur X/Y
  - Z + Haut/Bas : déplacer sur Z

### OBJ Editor

L'OBJ Editor est intégré dans XMTools. C'est un éditeur, pas une fenêtre externe.

Fonctionnalités :

- Ouvrir un mesh OBJ
- Conserver l'origine/pivot du fichier à l'ouverture
- Reset vers l'état original importé
- Center Auto pour centrer l'objet sur la grille
- Scale programmé
- Scale depuis un mesh de référence
- Scale x0.5
- Scale x2
- Sauvegarder en `.x`
- Sauvegarder en `.xm`
- Transformations non destructives jusqu'à l'export/sauvegarde
- Rendu OpenGL moderne avec grille
- Fenêtre d'aide avec icônes

Contrôles OBJ Editor :

Navigation :

- Clic gauche glissé : déplacer l'objet sur la grille X/Z
- Clic droit glissé : rotation de la vue
- Ctrl + clic gauche glissé : déplacement de la vue
- Molette souris : zoom caméra
- X + molette souris : scale de l'objet
- X + Gauche/Droite : réduire/agrandir l'objet

Mouvement :

- Flèches maintenues : déplacement continu sur X/Z
- Y + Haut/Bas : déplacer l'objet sur Y

Rotation :

- M + Gauche/Droite : rotation de l'objet sur X
- M + Haut/Bas : rotation de l'objet sur Y
- Z + Gauche/Droite : rotation de l'objet sur Z

Vue :

- R : reset transform
- V ou Home : vue diagonale haute

Scale :

- 1 : scale x0.5
- 2 : scale x2

Sauvegarde et aide :

- F5 : sauvegarder `.x`
- F6 : sauvegarder `.xm`
- H : afficher/masquer l'aide

### Options

Options SplashScreen :

- Choix du logo :
  - XboxToolsSuite 1
  - XboxToolsSuite 2
  - XboxToolsSuite 3
  - XboxToolsSuite 4
  - XboxToolsSuite 5
- Transparence :
  - Transparent Logo
  - No Transparency
- Redimensionner le logo pour le splash

Options XIP Tools :

- Ajout de fichiers :
  - Afficher uniquement les fichiers `.xap`, `.xm` et `.xbx`

Options XMTools :

- Import de mesh :
  - Ouvrir OBJ/X sans limite de vertices Xbox XM
- Limite XM :
  - Proposer le welding automatique des vertices lors d'une sauvegarde XM trop grande
- Couleur de l’overlay de référence :
  - Choisir la couleur utilisée pour l’overlay de référence dans l’Object Editor

Options des icônes de toolbar :

- Taille des icônes XIP Tools :
  - 32, 48, 64, 80, 96, 110, 128
- Taille des icônes XBX Tools :
  - 32, 48, 64, 80, 96, 110, 128
- Taille des icônes XMTools :
  - 32, 48, 64, 80, 96, 110, 128
- Taille des icônes Object Editor :
  - 32, 48, 64, 80, 96, 110, 128
