# 1. PRE-CALIBRATION

  1. Mesurer le spécimen à numériser;
  2. Ouvrir le logiciel *DISC3D*;
  3. Cliquer sur le menu **Optical setup** à gauche;
  4. Selon sa plus grande mensuration, sélectionner la configuration dont la valeur *Max. Object Size* est égale ou supérieure à cette dernière.

### Modifications matérielles sur le scanner

  5. Retirer les portes du scanner;
  6. Reculer la caméra à l’aide du bouton *Focus proche* sur le contrôleur DISC3D plus;
  7. Dévisser l’ensemble optique de la caméra;
  8. Consulter la charte d’optique afin de sélectionner les bons tubes d’extension, les bons anneaux, les bons adaptateurs et le bon objectif;
  9. Assembler les morceaux de l’ensemble optique (à noter que certaines parties de l’ensemble optique se vissent et dévissent ensemble; d’autres parties sont tenus par trois petites vis autour, qu’il faut enlever et remettre avec une mini clé Allen qui se trouve dans un petit sac en plastique);
  10. Consulter la charte de dôme d’éclairage pour savoir lequel est approprié; retirer et remplacer au besoin (parfois, il faut également changer le bloc de métal attaché au dôme; pour ce faire, il faut utiliser la clé Allen 2.5 (vert pâle));
  11. Revisser l’ensemble optique.

# 2. CALIBRATION

### De retour dans DISC3D

1. Toujours dans le menu **Optical setup**, sélectionner la configuration choisie et appuyer sur *Apply*;
2. Le logiciel demande de débrancher la caméra; débrancher le fil *USB3 - Caméra*, puis rebrancher immédiatement;
3. Au milieu en haut de l’interface, cliquer sur *Start live* pour voir l’image de la caméra en direct;
4. Mettre l’ouverture de l’objectif à la plus grande valeur possible (donc le chiffre le plus petit); il faut dévisser légèrement la petite vis noire sur l’objectif et aligner la ligne blanche avec la valeur désirée;
5. Dans le mandrin, insérer une sphère de pose de taille appropriée pour qu’elle ne dépasse pas le cadre de l’image; s’assurer qu’elle est grosso-modo au centre de l’image; sinon, ajuster la hauteur de la caméra avec les deux grosses vis noires vis-à-vis les colonnes (étiquetées *Translation vers le haut/bas*);
6. Une fois la sphère de pose relativement bien centrée, retirer du mandrin puis mettre le support pour matrice de calibration; il faut choisir la matrice appropriée selon la configuration choisie (l’information est indiquée sur la page présentement ouverte dans DISC3D - *Dot Pitch Target*);
7. S’assurer que la cible, une fois dans son socle, est elle aussi grosso modo au centre de l’image verticalement, mais cette fois-ci en ajustant la hauteur du socle et non celle de la caméra; il se peut que vous ayez besoin d’éloigner ou de rapprocher la caméra pour voir clairement la cible, dans ce cas utiliser les boutons sur le contrôleur physique du DISC3D;
8. Ajuster le *Exposure Time* et *Gain* de sorte que les points blancs de la cible paraissent en vert très pâle et soient légèrement surexposés;
9. Ajuster la position de la caméra avec les boutons du contrôleur physique de sorte à maximiser l’indicateur de netteté *Sharpness indicator*, accessible sur le côté droit de l’application;
10. Dévisser le petit bras du bloc noir situé au bas du rail (celui où il est écrit *Ajuster sur le point focal*), et le déplacer jusqu’à ce que la petite lumière orange qui y est accrochée soit à l’extrémité droite du morceau rouge (où il est écrit *Point focal*), juste assez pour s’allumer, puis reculer légèrement tout juste pour que la lumière orange s’éteigne;
11. Revisser le petit bras;
12. Cliquer sur *Done*, puis sur *Yes* si on vous demande si vous avez changé le système optique.
13. Ajuster l’ouverture de l’objectif pour qu’elle soit à son plus petit (donc le plus grand chiffre);
14. Ajuster le *Exposure Time* et *Gain* de sorte que les points blancs de la cible paraissent en vert très pâle et soient légèrement surexposés;
15. Une fois que tous les points sont verts et que la boîte de texte flottante affiche *Found 48 / 48*, ajuster la hauteur de la caméra (comme tout à l’heure) et la position gauche-droite (à l’aide des petites vis situées juste au dessus de la caméra, là où il est écrit *Translation vers la…*) de sorte à ce que la croix rouge du logiciel (bouton *Alignment* à droite) soit alignée avec la croix verte qui apparait être les points de la cible;
16. Appuyer sur *Start calibration*;
17. Une fenêtre *ANGLE ERROR* apparaît en haut à gauche : si les indicateurs sont à + ou - 0.05, sautez à l'étape **2.21**. Sinon, pour ajuster la valeur horizontale, ajuster les petites vis jaunes qui se trouvent derrière le rail motorisé (nommées *Droite* et *Gauche*), et pour la valeur horizontale, ajuster les petites vis jaunes plus hautes (nommées *Haut* et *Bas*). Pour serrer une vis, il faut desserrer celle du côté opposé;
18. Ensuite, ajuster la hauteur et la translation gauche-droite de la caméra pour que la croix rouge soit à nouveau alignée à la croix verte;
19. Appuyer sur *Recalibrate*, puis *Start calibration*;
20. Répéter les étapes **2.16** à **2.19** autant de fois que nécessaire.
21. Tout est ok et vous pouvez cliquer sur *Accept*.

# 3. NUMÉRISATION

1. Mettre l’ouverture à F5.6;
2. Cliquer sur le menu **Scan** à gauche;
3. Dans l’onglet **Imaging**, mettre le *Frontlight* à 50%, et le *Backlight* à 100%;
4. Ajuster le *Exposure Time* et *Gain* pour que le spécimen soit bien éclairé mais pas saturé;
5. Ne rien changer dans l’onglet **Image Processing** (tout doit être à off);
6. Dans l’onglet **3D Scan**, dans *Pose Programs*, choisir *360 deg delta = 10 deg*;
7. Dans *Azimuth Release Time* et *Elevation Release Time*, mettre 2 sec;
8. Dans *Directory*, choisir le dossier où vous souhaitez sauvegarder votre scan;
9. Dans *Name*, copier-coller le nom du dossier;
10. Ferme les portes du scanneur;
11. Appuyer sur *Start scan*.

# 4. RENOMMER LES PHOTOS EN VUE DU TRAITEMENT

1. Copier-coller le dossier *edof* et le renommer *edof_renamed*.

### Dans Advanced Renamer

2. Ajouter toutes les photos du dossier *edof_renamed*
3. Ajouter la méthode **Remove**, avec les paramètres suivants :
    - *Remove type* : ***Position***
    - *Starting at* : ***11***
    - *Count* : ***12 (ou plus)***
    - *Backwards* : ***off***
    - *Case sensitive* : ***off***
    - *Use regular expressions* : ***off***
    - *Apply to* : ***Name***
4. S’assurer que le *Batch mode* est à *Rename*
5. Cliquer sur *Start batch*.

# 5. TRAITEMENT DES PHOTOS

### Dans Davinci Resolve

1. Créer un nouveau projet;
2. Aller dans l’onglet **Media**;
3. Dans le navigateur de fichiers, trouver le dossier des photos précédemment renommées (*edof_renamed*);
4. Cliquer sur les trois points en haut à droite de la fenêtre de recherche de fichiers, sélectionner *Frame display mode -> Sequence*;
5. Glisser la séquence d’image dans le *Media pool*;
6. Aller dans l’onglet **Edit**;
7. Sélectionner la séquence d’images et la glisser-déposer dans la timeline;
8. Cliquer sur la roue dentée en bas à droite de l’interface, ce qui ouvre les paramètres de projet. Dans *Timeline resolution*, aller tout en haut et choisir *Custom*. Puis juste en dessous, écrire *4096 x 3008*, puis cliquer sur *Save* en bas à droite de la page;
9. Aller dans l’onglet **Fusion**;
10. Ouvrir le menu *Effects* en haut à droite;
11. Cliquer sur le bouton loupe, chercher *Delta Keyer*;
12. Placer entre *MediaIn* et *MediaOut*;
13. Cliquer sur *Background color* à droite, puis *Pick screen color* pour sélectionner la couleur de la couleur de fond. Sinon, notez la valeur hexadécimale quand vous placez le curseur sur le fond;
14. Dans les options de **Delta Keyer**, ajuster les valeurs *Red*, *Green* et *Blue* à droite pour minimiser les couleurs de fonds et maximiser la préservation des détails;
15. Dans les effets, chercher *Color Corrector* et ajouter à la chaîne d'effets;
16. Ajuster le *gamma* et la *saturation*, ainsi que le *hue* si nécessaire;
17. Dans les effets, chercher *Sharpen* et ajouter à la chaîne d'effets;
18. Ajuster légèrement (généralement, entre 0.1 et 0.2);
19. Cliquer sur l’onglet **Deliver**;
20. Cliquer sur *Browse* à droite de *Location* pour choisir le dossier où vous souhaitez exporter les photos (idéalement, un dossier nommé *edof_exported*)
21. À la ligne *Render*, choisir *Individual clips*
22. Juste en dessous, dans l’onglet **Video**, choisir :
    - *Format* : ***PNG***
    - *Codec* : ***RGB 8 bits***
    - *Render at source resolution* : ***yes***
    - *Export alpha* : ***yes***
    - *Alpha* : ***Premultiplied***
    - *Compression level* : ***0***
    - *Advanced settings*
      - *Data levels* : ***Full***
23. Cliquer sur l’onglet **File** qui est à droite de *Audio* et *Video* un peu plus haut :
    - *Filename uses* : Source name
    - *Use … digits in the filename* : 1
    - Cliquer sur *Add to Render Queue*
24. En haut à droite, dans la fenêtre **Render Queue**, cliquer sur *Render All*;
25. Si les photos sont bien exportées, effacer le dossier *edof_renamed*.

# 6. RENOMMER LES PHOTOS APRÈS L'EXPORTATION

### Dans Advanced Remamer

1. Importer les photos du dossier *edof*;
2. Sélectionner tous les fichiers dans la liste;
3. Clic-droit, **Export**, puis dans la fenêtre qui s’ouvre : 
    - *Format* : ***Text***
    - *Filename* : cliquer sur les trois petits points pour déterminer le dossier où le fichier sera enregistré, et indiquer un nom de fichier (*edof_filenames*)
    - *File encoding* : ***UTF-8***
    - *Export field* : ***Filename***
4. Fermer Advanced Renamer, réouvrir;
5. Importer les photos du dossier *edof_exported*;
6. Ajouter comme méthode **List** :
    - Dans *List*, cliquer sur *Load list*, et sélectionner le fichier texte exporté précédemment
    - *Apply to* : ***Name***
7. Ajouter comme méthode **Remove pattern** :
    - “Pattern” : .png
8. *Batch mode* (en haut au milieu de l’interface) : ***Rename***
9. Cliquer sur *Start batch*.

# 7. MODÉLISATION

### Dans Metashape (v2.2.2)

1. Ouvrir l’onglet “Reference” en bas à gauche de l’interface, puis le bouton “Settings” (Marteau et clé anglaise)
2. Dans la fenêtre qui s’ouvre, dans “Coordinate System”, choisir “Custom”
3. Dans l’autre fenêtre qui s’ouvre, cliquer sur le bouton “Load” (la filière) puis sélectionner le fichier “local-coordinates-mm.prj”
4. Onglet “Workflow”, “Add folder”, sélectionner le dossier “edof_exported”
5. Dans la fenêtre qui s’ouvre, “Please select data layout : Single cameras”

### Option 1 : Si vous avez accès à un fichier “Pose_Sphere_XX_Cameras.xml” pour la configuration choisie : 

6. Menu “File”, “Import”, “Import cameras”, sélectionner le fichier .xml dans le dossier de Pose Sphere qui correspond à l’échelle de photographie utilisée (ex. si vous utilisez l’échelle XS avec un stepsize de 10 entre les photos, sélectionnez le fichier qui contient dans son nom “PoseSphere-XS_step10”; ce fichier se trouve dans un dossier éponyme dans le dossier des scans
7. Dans la fenêtre qui s’ouvre :
8. Accuracy : Highest
9. Generic preselection : oui
10. Reference preselection : oui
11. Keypoint limit : 250 000
12. Tie point limit : 250 000
13. Guided image matching : non
14. Exclude stationary tie points : oui
15. Menu “Tools”, “Optimize cameras”, cocher “Fit f” seulement

### Option 2 : Si vous n’avez PAS accès à un fichier “Pose_Sphere_XX_Cameras.xml” pour la configuration choisie : 

16. Ouvrir le fichier “ScanInformation.pdf”
17. Copier la valeur à la ligne “2.4. Camera Constant/f [px]:”
Menu “Tools”, “Camera Calibration”
Dans la fenêtre qui s’ouvre : 
Changer “Mode : Auto” à “Precalibrated”
Coller la valeur “Camera Constant/f” à la ligne “f”
Bouton “Fixed Parameters”, cocher “Check all” puis décocher “f”; fermer la fenêtre
Appuyer sur Ok
Menu “File”, “Import”, “Import Reference”
Dans la fenêtre qui s’ouvre : 
S’assurer que le champ “Coordinate system” est à “Local coordinates (mm)”
“Delimiter” est à “Space”
“Column Labels” sont à “1”, “2”, “3” et “4”
Décocher “Accuracy” et “Rotation”
Ok
Menu “Workflow”, “Align Photos”
Dans la fenêtre qui s’ouvre : 
Accuracy : Highest
Generic Preselection : Oui
Reference Preselection : Oui, “Source” (si cette option est grise, c’est que vos photos sont mal nommées; revoir les étapes de renommage)
Advanced : 
Key Point Limit : 250,000
Tie Point Limit : 250,000
Exclude Stationary Points : Oui
Guided Image Matching : Non
Adaptive Camera Model Fitting : Non
Menu “Tools”, “Optimize cameras”, cocher “f” seulement. Refaire au besoin si le nuage de points a l’air flou

Suite : 

À droite du bouton de sélection, deux boutons à droite du bouton avec une flèche, sélectionner “Resize region”
Ajuster la taille du bloc pour contenir tout juste le spécimen
Sélectionner l’onglet “Workspace” en bas à gauche de “Reference”, clique-droit sur “Chunk1”, “Duplicate” (je ne sais pas pourquoi cette étape, mais faites-le quand même)
Menu “Tools”, “Tie Points”, “Clean Tie Points”
Dans la fenêtre qui s’ouvre : 
Criterion : Reprojection Error
Dans la fenêtre d’affichage 3D, vous voyez un chiffre en bas à gauche, soit le nombre de Tie points. Juste à droite de ce chiffre, un autre chiffre qui montre le nombre de Tie points sélectionnés
Dans le champs “Level”, mettre le curseur à un endroit où le nombre de Tie points sélectionnés correspond à environ 10% du nombre total de Tie points
Ok
Supprimer les points
Deuxième fois, Menu “Tools”, “Tie Points”, “Clean Tie Points”
Dans la fenêtre qui s’ouvre : 
Criterion : Projection accuracy
Le reste idem
Ok
Supprimer les points
Menu “Workflow”, “Build Model”
Dans la fenêtre qui s’ouvre : 
Source data : Depth maps
Quality : Ultra high
Face count : High
Dans la section “Advanced” : 
Interpolation : Enabled
Depth filtering : Mild
Calculate vertex color : oui
Menu “Tools”, “Model”, “Clean model”
Dans la fenêtre qui s’ouvre : 
Criterion : Connected Component Size
Level : 99
Ok
Cliquer sur l’outil de sélection et entourer les bouts à enlever (ex. l’aiguille) et supprimer
Menu “Tools”, “Close holes”
Dans la fenêtre qui s’ouvre, cliquer sur Ok
Menu “Workflow”, “Build Texture”
Dans la fenêtre qui s’ouvre : 
Texture type : Diffuse map
Source data : Images
Mapping mode : Generic
Blending mode : Mosaic
Texture size : 8192
Page count : 1
Enable hole filling : yes
Enable ghosting filter : yes
Menu “Workflow”, “Build Point Cloud”
Dans la fenêtre qui s’ouvre : 
Source data : Depth maps
Quality : Ultra high
Reuse depth maps : oui
Save project after each step : non
Depth filtering : Mild
Calculate point colors : oui
Calculate point confidence : oui
Sauvegarder le projet Metashape.


EXPORTATIONS ET TRAITEMENTS DES DONNÉES

Dans Metashape

Menu “File”, “Export”, “Export Point Cloud”
Choisir le type de fichier “Stanford PLY” puis nommer le fichier en lui donnant le suffixe “_HIGH”
Dans la fenêtre qui s’ouvre : 
Coordinate System : Local Coordinates (mm)
Convert color to 8 bit RGB : oui
Binary encoding : oui
Color : oui
Normal : oui
Classification : oui
Confidence : oui
Menu “File”, “Export”, “Export Cameras”
Choisir le type de fichier “Colmap” puis nommer le fichier en lui donnant le suffixe “_COLMAP”
Dans la fenêtre qui s’ouvre : 
Coordinate System : Local Coordinates (mm)
Images : non
Tie points : oui
Transform to pinhole camera : non
Transform to initial calibration : non
Binary encoding : oui
Masks : non
Control points
Image name template : {filename}_{filenum}.png
Fermer Metashape

Dans Cloud Compare

Ouvrir le fichier “(...)_HIGH.ply” avec Cloud Compare
Dans le fenêtre qui s’ouvre, cliquer sur “Apply”
Sélectionner le modèle importé, dans la fenêtre de gauche
Cliquer sur le bouton “Subsample a point cloud” (amas de points)
Dans la fenêtre qui s’ouvre : 
method : Octree
subdivision level : 11
Ok
Cliquer sur le bouton “Save current entity” (disquette), aller dans le dossier du projet, nommer “(...)_LOW.ply”, Save, puis cliquer sur “BINARY”
Fermer Cloud Compare

Dans Colmap

Aller dans le dossier “colmap-x64-windows-cuda” qui se trouve dans le dossier racine des projets de scan
Clic-droit sur le fichier “COLMAP.bat”, “Run as administrator”
Menu “File”, “Import model from”
Sélectionner le fichier “(...)_LOW.ply” précédemment créé
Menu “File”, “Export model”
Dans la fenêtre ouverte, créer un dossier “colmap” et sélectionner
Fermer Colmap

Dans le dossier du projet

Aller dans le dossier “colmap”
Copier le fichier “points3D.bin”
Aller dans le dossier “sparse”, “0”
Coller-remplacer le fichier “points3D.bin”

RENOMMAGE DES PHOTOS POUR POSTSHOT

Créer un dossier “edof_exported_renamed”

Dans Advanced Renamer

Charger les photos du dossier “edof_exported”
Ajouter comme méthode “Add”
Dans le champ “Add:”, écrire “_<Inc Nr:0>
Dans le champ “At index:”, écrire “0”
Cocher “Backwards”
Ne pas cocher “Use regular expressions”
“Apply to: Name”
“Batch mode” (en haut au milieu de l’interface) : Copy
“Output folder” : le dossier “edof_exported_renamed”
Cliquer sur “Start batch”
Fermer Advanced Renamer

GÉNÉRATION DU GAUSSIAN SPLAT

Dans Postshot

Glisser-déposer les dossiers “sparse” et “edof_exported”
Dans la fenêtre ouverte : 
Image selection : Use All Images
Camera Poses : Import
Radiance Field Profile : Splat3
Limit Image Size : oui, 3840
Max Splat Count : 3000
Anti-Aliasing : non
Start Training : oui
Stop Training after : oui, 30 kSteps
Cliquer sur “Import”
Une fois le training terminé, à l’aide du bouton de rotation à gauche et de la souris, ajuster le spécimen pour qu’il soit droit (à l’endroit) vis-à-vis de la fenêtre
Menu “File”, “Export Scene Rdnc Field”
Nommer le fichier “(...)_RADIANCE-FIELD.py”




