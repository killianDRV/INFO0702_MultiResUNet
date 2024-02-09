# DRV Killian - Projet INFO0702

## Données médicales
- site du [ISIC-2017_Data](https://challenge.isic-archive.com/data/#2017)
    - **train :**
        - [training image](https://isic-challenge-data.s3.amazonaws.com/2017/ISIC-2017_Training_Data.zip)
        - [mask image](https://isic-challenge-data.s3.amazonaws.com/2017/ISIC-2017_Training_Part1_GroundTruth.zip)
    - **test :**
        - [test image](https://isic-challenge-data.s3.amazonaws.com/2017/ISIC-2017_Test_v2_Data.zip)
        - [mask image](https://isic-challenge-data.s3.amazonaws.com/2017/ISIC-2017_Test_v2_Part1_GroundTruth.zip)

<br>

**A la racine :**
```
ISIC-2017_Data/
├── test/  # Images pour le test
│   ├── images/  # Images pour le test
│   │   ├── ISIC_0012086.jpg
│   │   ├── ISIC_0012092.jpg
│   │   ├── ISIC_0012095.jpg
│   │   ...
│   │
│   └── masks/  # Masks pour le test 
│       ├── ISIC_0012086.png
│       ├── ISIC_0012092.png
│       ├── ISIC_0012095.png
│       ...
│
└── train/  # Images pour le train
    ├── images/  # Images pour le train
    │   ├── ISIC_0000000.jpg
    │   ├── ISIC_0000001.jpg
    │   ├── ISIC_0000002.jpg
    │   ...
    │
    └── masks/  # Masks pour le train 
        ├── ISIC_0000000.png
        ├── ISIC_0000001.png
        ├── ISIC_0000002.png
        ...
```

## Données des plantes
- [leaf image](https://drive.google.com/drive/folders/1_0cnT6K9tim96dHPeWNjjPAZbgzqIFuD)

<br>

**A la racine :**
```
plantDoc_leaf_disease/
├── aug_data/  # Contient les images de la base `augmented_data`
│   ├── test/  # Base pour le test de `augmented_data`
│   │   ├── images/  # Image pour le test
|   |   |   ├── 00000_1.jpg
|   |   |   ├── 00000_3.jpg
|   |   |   ├── 00002_1.jpg
|   |   |   ...
|   |   |
│   |   └── masks/  # Masks pour le test 
|   |       ├── 00000_1.png
|   |       ├── 00000_3.png
|   |       ├── 00002_1.png
|   |       ...
|   |
│   └── train/  # Base pour le train de `augmented_data`
│       ├── images/  # Image pour le train
|       |   ├── 00000_0.jpg
|       |   ├── 00000_2.jpg
|       |   ├── 00000_4.jpg
|       |   ...
|       |
│       └── masks/  # Masks pour le train 
|           ├── 00000_0.png
|           ├── 00000_2.png
|           ├── 00000_4.png
|           ...
|
└── data/  # Contient les images de la base `data`
    ├── test/  # Base pour le test de `data`
    │   ├── images/  # Image pour le test
    |   |   ├── 00000.jpg
    |   |   ├── 00000_3.jpg
    |   |   ├── 00002_1.jpg
    |   |   ...
    |   |
    |   └── masks/  # Masks pour le test 
    |       ├── 00000_1.png
    |       ├── 00000_3.png
    |       ├── 00002_1.png
    |       ...
    |
    └── train/  # Base pour le train de `data`
        ├── images/  # Image pour le train
        |   ├── 00004.jpg
        |   ├── 00010.jpg
        |   ├── 00022.jpg
        |   ...
        |
        └── masks/  # Masks pour le train 
            ├── 00004.png
            ├── 00010.png
            ├── 00022.png
            ...
```
## Test du programme
- **Demo.ipynb** permet de tester avec les données des plantes
- **Demo_original_data.ipynb** permet de tester avec les données d'origine (données médicales)

## Résultat
Les prédictions sont stockées dans le dossier `results`
```
plantDoc_leaf_disease/
├── aug_data/  # Prédiction sur la base de plante augmentée
│   ├── 0.png
│   ├── 1.png
│   ├── 2.png
│   ...
│
├── data/  # Prédiction sur la base de plante
│   ├── 0.png
│   ├── 1.png
│   ├── 2.png
│   ...
│
└── original_data/  # Prédiction sur la base d'origine
    ├── 0.png
    ├── 1.png
    ├── 2.png
    ...
```