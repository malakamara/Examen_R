
# Analyse Statistique des Données AVC

## Description du projet

Ce projet présente une analyse statistique complète des données d'Accident Vasculaire Cérébral (AVC). L'objectif est d'explorer les caractéristiques démographiques, cliniques et évolutives d'une cohorte de patients ayant subi un AVC, afin d'identifier les facteurs de risque, d'évaluer la sévérité des événements et d'analyser l'efficacité des traitements.

## Structure du projet

```
querto/
├── analyse_avc.qmd          # Document Quarto principal
├── _quarto.yml              # Configuration Quarto
├── dataAVC.csv              # Données source
├── README.md                # Ce fichier
└── docs/                    # Dossier de sortie (généré)
```

## Prérequis

### Logiciels nécessaires

- **R** (version 4.0 ou supérieure)
- **Quarto** (version 1.0 ou supérieure)
- **RStudio** (recommandé, mais optionnel)

### Packages R requis

Les packages suivants seront installés automatiquement lors de l'exécution :

- `tidyverse` : Manipulation et visualisation de données
- `ggplot2` : Création de graphiques
- `corrplot` : Visualisation de matrices de corrélation
- `gridExtra` : Organisation de graphiques multiples
- `lubridate` : Manipulation de dates

## Installation

1. **Installer R** : Télécharger depuis [CRAN](https://cran.r-project.org/)

2. **Installer Quarto** : Télécharger depuis [Quarto.org](https://quarto.org/docs/get-started/)

3. **Cloner ou télécharger ce projet**

4. **Vérifier que le fichier `dataAVC.csv` est présent** dans le répertoire du projet

## Utilisation

### Compiler le document Quarto

#### Méthode 1 : Via RStudio

1. Ouvrir `analyse_avc.qmd` dans RStudio
2. Cliquer sur le bouton "Render" ou utiliser `Ctrl+Shift+K` (Windows/Linux) ou `Cmd+Shift+K` (Mac)

#### Méthode 2 : Via la ligne de commande

```bash
quarto render analyse_avc.qmd
```

### Formats de sortie

Le document peut être compilé en plusieurs formats :

- **HTML** : `quarto render analyse_avc.qmd --to html`
- **PDF** : `quarto render analyse_avc.qmd --to pdf`
- **Word** : `quarto render analyse_avc.qmd --to docx`

Les fichiers générés seront placés dans le dossier `docs/`.

## Structure du rapport

Le rapport est organisé en sections principales :

1. **Configuration et Import des données**
   - Chargement des packages
   - Import des données
   - Préparation et nettoyage

2. **Statistiques descriptives**
   - Caractéristiques démographiques
   - Facteurs de risque
   - Analyses par sexe

3. **Analyses cliniques**
   - Distribution du NIHSS
   - Délai de consultation
   - Paramètres biologiques

4. **Tests statistiques**
   - Comparaisons de moyennes
   - Tests de corrélation
   - Analyses multivariées

5. **Traitements et évolution**
   - Traitements administrés
   - Évolution dans le temps
   - Pronostic

## Résultats principaux

### Caractéristiques de l'échantillon

- **Nombre de patients** : 875
- **Âge moyen** : 64.3 ± 13 ans
- **Sexe ratio H/F** : 1.83

### Facteurs de risque

- **HTA** : 60.1%
- **Diabète** : 49.0%
- **Tabac** : 29.2%

### Sévérité et évolution

- **NIHSS initial moyen** : 6.85
- **NIHSS sortie moyen** : 5.43
- **Amélioration moyenne** : 1.35 points
- **Taux de mortalité** : 3.9%

## Personnalisation

### Modifier les paramètres de sortie

Éditer le fichier `_quarto.yml` pour personnaliser :

- Le thème HTML
- Les paramètres PDF
- Les options d'exécution du code
- La numérotation des sections

### Ajouter des sections

Le fichier `analyse_avc.qmd` peut être modifié pour ajouter :

- De nouvelles analyses
- Des graphiques supplémentaires
- Des interprétations détaillées

## Dépannage

### Erreur : Package non trouvé

Si un package R n'est pas trouvé, exécuter dans R :

```r
install.packages("nom_du_package")
```

### Erreur : Fichier de données non trouvé

Vérifier que `dataAVC.csv` est dans le même répertoire que `analyse_avc.qmd`.

### Erreur : Quarto non trouvé

Vérifier l'installation de Quarto :

```bash
quarto --version
```

Si Quarto n'est pas installé, suivre les instructions sur [Quarto.org](https://quarto.org/docs/get-started/).

## Contribution

Pour contribuer à ce projet :

1. Créer une branche pour vos modifications
2. Tester vos changements
3. Soumettre une pull request

## Licence

Ce projet est fourni à des fins éducatives et de recherche.

## Contact

Pour toute question ou suggestion, veuillez ouvrir une issue sur le dépôt du projet.

## Références

- [Documentation Quarto](https://quarto.org/docs/)
- [Documentation R](https://www.r-project.org/help.html)
- [Tidyverse](https://www.tidyverse.org/)


