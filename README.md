# Cartes de Révision en Markdown pour Anki

Ce projet fournit des fichiers markdown contenant des concepts de 
mathématiques et d'informatique, structurés selon un format spécifique. 
Ces fichiers peuvent être transformés en cartes Anki à l'aide du [_fork_](https://github.com/titusse3/mdanki).

## Table des matières
1. [Description du Projet](#Description-du-Projet)
2. [Prérequis](#Prérequis)
3. [Installation](#Installation)
4. [Licence](#Licence)

## Description du Projet

Ce projet vise à faciliter la révision et l'apprentissage des concepts 
de la théorie des catégories, d'informatique et même de mathématique en 
fournissant des fichiers _Markdown_ sous un format spéciale. Les 
fichiers _Markdown_ sont conçus pour être compatibles avec 
[mdankiFork](https://github.com/titusse3/mdanki.git), qui permet de convertir 
ces fichiers en cartes _Anki_ pour une révision efficace.

## Prérequis

- [Node.js](https://nodejs.org)
- [mdankiFork](https://github.com/titusse3/mdanki.git)

## Installation

1. Clonez et installez le fork de __mdanki__ :
```bash
git clone https://github.com/titusse3/mdanki.git
cd mdanki
npm i -g
```

2. Clonez ce dépôt sur votre machine locale :
```bash
git clone https://github.com/titusse3/ankiCardPerso.git
cd ankiCardPerso
```

3. Conversion en paquet _Anki_ des fichiers fourni :
```bash
mdanki content nom_du_fichier.apkg
```

4. importer le paquet `.apkg` dans _Anki_.

## Licence

Ce projet est sous licence GPLv3. Consultez le fichier [LICENSE](LICENSE) pour 
plus de détails.