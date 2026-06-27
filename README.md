# Steam — Analyse de la marketplace du jeu vidéo

Analyse exploratoire en big data du catalogue Steam pour orienter la stratégie de sortie d'un nouveau jeu.

Projet de certification Jedha — Data Science, bloc #2.

## Contexte

Un éditeur (Ubisoft) veut lancer un nouveau titre et cherche, à partir des données du marché, la meilleure stratégie : genre, prix, langues, plateformes et timing de sortie.

## Dataset

- 55 691 jeux
- 22 variables (éditeur, genre, prix, plateformes, avis, dates de sortie)
- Source : catalogue Steam, fichier JSON semi-structuré stocké sur S3

## Méthode

Traitement distribué en **PySpark sur Databricks** : aplatissement du JSON imbriqué, cast des types, puis analyses univariées et multivariées.

## Contenu du repo

```
.
├── notebooks/
│   └── Steam_project.ipynb
├── steam-videogames-platform.html
└── README.md
```

## Principaux résultats

- Le volume n'est pas le succès : les plus gros éditeurs sont des spécialistes du casual, pas les studios AAA.
- Prix moyen du marché à 7,73 € (tiré vers le bas par l'indé) ; le segment premium est peu encombré.
- Combo gagnant Action + Adventure : du volume et la meilleure satisfaction (Adventure 77,7 %).
- Cinq langues prioritaires (anglais, allemand, français, russe, chinois simplifié) couvrent 90 % du marché.

Détails et interprétations dans le notebook.

## Auteur

Ramili Rindra — Jedha - DSFS, 2026.
