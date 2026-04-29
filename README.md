# 📘 Théorie des Distributions — Exposé MMI 2

Ce dépôt contient le code source \LaTeX\ complet pour un exposé portant sur la **Théorie des Distributions**. Ce document a été rédigé dans le cadre du cours de **M**éthode **M**athématique de l'**I**ngénieur II (MMI 2).

* **Auteurs :** Parfait BOTCHI, Judikael DOBOEVI, Prosper AFFOUKOU, Alexis DOHOU
* **Institution :** ENSGMM (École Nationale Supérieure de Génie Mathématique et Modélisation) – UNSTIM
* **Niveau/Public :** Ingénieur 1Génie Mathématique et Modélisation
* **Design du document :** Élégant, monochrome (noir/blanc/nuances de gris) .

---

## 📑 Table des matières
- [📘 Théorie des Distributions — Exposé MMI 2](#-théorie-des-distributions--exposé-mmi-2)
  - [📑 Table des matières](#-table-des-matières)
  - [🧠 Contenu du document](#-contenu-du-document)
  - [🎨 Aperçu visuel et Typographie](#-aperçu-visuel-et-typographie)
  - [📂 Structure du projet](#-structure-du-projet)
  - [⚙️ Prérequis](#️-prérequis)
  - [🚀 Compilation](#-compilation)
  - [✏️ Personnalisation](#️-personnalisation)
  - [©️ Licence et Droits d'auteur](#️-licence-et-droits-dauteur)

---

## 🧠 Contenu du document

Le recueil traite des concepts fondamentaux de la mécanique et de la modélisation mathématique s'appuyant sur les *distributions*, avec entre autres :
- Introduction et formalismes mathématiques.
- Outils d'analyse fonctionnelle.
- La **distribution de Dirac** (Impulsion de Dirac).
- Applications pratiques aux **Équations aux Dérivées Partielles (EDP) Linéaires**.
- Méthodes et corrections d'exercices d'application (section 7).

---

## 🎨 Aperçu visuel et Typographie

Le document se distingue par un template \LaTeX\ extrêmement soigné, conçu pour une lisibilité parfaite sur papier et sur écran :
- **Polices :** Palatino (`mathpazo` pour le texte et les mathématiques) procurant une élégance classique.
- **Couleurs :** Monochromatique académique (nuances de gris : `titlegray`, `theorembar`, `shadedef`, etc.).
- **En-têtes et Pieds de page :** Mis en forme avec le package `fancyhdr` pour un repérage rapide.
- **Page de couverture :** Design élaboré et géométrique entièrement codé en `TikZ` (boucles, tracés fluides, teintes or et bleu marine pour l'identité UNSTIM).
- **Théorèmes et Définitions :** Boîtes encadrées élégantes avec bordure latérale via `mdframed`.

---

## 📂 Structure du projet

Voici un descriptif des éléments essentiels du répertoire :

```text
├── main.tex                 # Fichier maître consolidant tout le projet (à compiler)
├── main_updated (1).tex      
├── titlepage.tex            # Code source dédié purement à la somptueuse page de garde (TikZ)
├── espose_section_7.tex    
├── 1 et 2 MMI 2.txt         # Brouillons, notes ou textes préparatoires
├── *.aux, *.lof, *.toc      # Fichiers auto-générés par la compilation LaTeX
└── README.md                # Ce manuel de présentation
```

---

## ⚙️ Prérequis

Pour compiler harmonieusement le projet en local, une distribution \LaTeX\ complète est recommandée, telle que :
- [TeX Live](https://tug.org/texlive/) (Windows/Linux/Mac)
- [MiKTeX](https://miktex.org/) (Windows)
- [MacTeX](https://tug.org/mactex/) (macOS)

Les **packages LaTeX principaux** requis sont standard, mais assurez-vous d'avoir : `mathpazo`, `geometry`, `mdframed`, `fancyhdr`, `titlesec`, `tikz` (avec les librairies `shadings`, `calc`), `hyperref` et les paquets de l'AMS (`amsmath`, `amssymb`, `amsthm`).

---

## 🚀 Compilation

1. Ouvrez votre terminal ou invite de commande.
2. Naviguez vers le dossier racine contenant les fichiers du projet.
3. Exécutez `pdflatex` (deux ou trois fois pour générer correctement la table des matières `*.toc` et synchroniser les hyperliens) :

```bash
pdflatex main.tex
pdflatex main.tex
```

Vous pouvez aussi utiliser `latexmk` pour automatiser la couverture des dépendances :
```bash
latexmk -pdf main.tex
```
*(Note : Si vous utilisez un éditeur de code tel que **VS Code (avec l'extension LaTeX Workshop)**, **TeXstudio** ou **Overleaf**, la compilation se fera en un seul clic !)*

---

## ✏️ Personnalisation

Si vous souhaitez modifier et réutiliser ce template :
- **Couleurs :** Dans le préambule de `main.tex`, modifiez les variables `\definecolor` (ex: `shadedef`, `shadethm`) pour ajuster le gris ou passer en couleur RVB.
- **Identité :** Allez dans `titlepage.tex` pour éditer les couleurs de l'école (`unstimPrimary`, `unstimAccent`) et le nom de l'auteur.

---

## ©️ Licence et Droits d'auteur

Ce projet et ce document LaTeX appartiennent à **BOTCHI Parfait** (ENSGMM/UNSTIM). 
Le présent code peut servir de source d'inspiration pour vos travaux de composition \LaTeX\, en conservant crédit à son auteur.
