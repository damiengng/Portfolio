---
title: CloneWar
publishDate: 2023-09-21 00:00:00
img: /assets/clonewar.jpeg
img_alt: clonewar image
description: |
  Écrire une application web qui analyse des fichiers jar pour détecter des codes communs .
tags:
  - Dev
---

#### Présentation

Le but du projet CloneWar est d'écrire une application web qui analyse des fichiers jar (Java Archive) pour détecter des codes communs (on parle de clones).  
L'application CloneWar est composée d'un back-end écrit en Java offrant différents services REST permettant d'accéder aux informations de l'analyse d'une archive et d'un front-end écrit en JavaScript affichant ces informations et en particulier les codes sources considérés comme des clones.  
Ces deux composants sont reliés grâce à Quarkus pour le back-end et Angular pour le front-end.  


La première étape importante a été d'établir des connexions solides entre le back-end et le front-end.  
Les services REST fournis par le back-end permettent au front-end d'accéder facilement aux informations résultant de l'analyse des archives JAR, y compris les sections de code identifiées comme des clones.  

De plus, il était essentiel de mettre en place des connexions entre le back-end et la base de données.  
Dans ce projet, Quarkus a été utilisé avec la base de données H2.  
Pour faciliter la gestion de la base de données, un fichier "import.sql" a été développé, permettant ainsi de modifier directement la base de données à partir du projet.  

Le front-end a été conçu pour afficher de manière efficace les données récupérées.   Il a été configuré pour gérer la connexion, utiliser des requêtes SQL pour récupérer les informations pertinentes, puis les afficher.  
Tailwind a été utilisé pour améliorer l'aspect visuel de l'application, offrant ainsi une expérience utilisateur agréable.  

Enfin, l'application a été enrichie de fonctionnalités permettant aux utilisateurs d'ajouter facilement des fichiers JAR directement depuis leur ordinateur.   L'algorithme de Karp-Rabin a été implémenté pour effectuer l'analyse comparative des fichiers et détecter les clones de manière précise et efficace.
