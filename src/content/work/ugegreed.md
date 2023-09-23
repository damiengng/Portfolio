---
title: UGEGreed
publishDate: 2023-09-20 00:00:00
img: /Portfolio/assets/tcp.jpeg
img_alt: tcp image
description: |
  Réaliser un système de calcul distribué en utilisant le protocole TCP.
tags:
  - Dev
---

Le projet UGEGreed a pour objectif de réaliser un système de calcul distribué en utilisant le protocole TCP.  
L’idée est d’aider les chercheurs à tester des conjectures sur un grand nombre de cas en répartissant la tâche de vérification sur plusieurs machines.  
En général, pour tester une conjecture sur tous les nombres d'une plage donnée, les chercheurs écrivent une fonction Java qui vérifie la conjecture pour chaque nombre de la plage.  
Cependant, cela peut prendre beaucoup de temps, donc UGEGreed permettra de distribuer la vérification sur plusieurs machines en partageant les tâches à effectuer.   
Le but de ce projet est de concevoir un protocole et de rédiger une RFC (Request for Comments) pour ce dernier, puis de coder l'application suivant ce protocole.   

Plusieurs aspects cruciaux de ce projet comprennent la gestion des arguments, la création de classes dédiées pour la gestion du serveur et du client, l'établissement de connexions entre serveurs et clients, l'utilisation de fichiers JAR pour faciliter les opérations, la gestion des trames de données et la mise en place d'une table de routage pour assurer une distribution efficace des tâches.


