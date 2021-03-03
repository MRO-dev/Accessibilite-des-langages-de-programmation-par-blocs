# Accessibilite-des-langages-de-programmation-par-blocs
Le projet ci-après a pour objectif de rendre accessible par des non-voyants l’utilisation d’un langage de programmation par blocs de type Scratch. 

Ce dispositif comporte des objets tangibles représentant les différents blocs et les différentes variables et un logiciel automatique de reconnaissance de ces objets permettant de générer et d’exécuter le programme conçu par l’utilisateur.

La solution proposée comprend deux aspects.
Il s’agit d’une part de proposer un système permettant la manipulation physique de briques en bois représentant les blocs de base du langage Scratch. Ces pièces, une fois assemblées, forment un algorithme qui est interprété par un ordinateur à l’aide d’outils de reconnaissance visuelle.
Le deuxième enjeu est d’intégrer des outils d’interaction (robots, sorties tactiles ou sonores) rendant l’exécution des algorithmes compréhensibles pour un utilisateur non-voyant. Ce deuxième enjeu n'a pas été complètement implémenté.

Le programme principal du projet (situé sous IntegrationGlobale\src\main\java\Assemblage\CreationScratch.java) prend en entrée un cliché de l'algorithme réalisé physiquement en Scratch (disponible sous ClichesAlgorithmes/Algorithme.jpg) et un fichier ScratchOriginal.zip comprenant la structure d'un programme écrit en Scratch et stocké au format JSON. 
La méthode principale implémente un algorithme de reconnaissance qui transforme un cliché d'un algorithme Scratch en un projet Scratch 3.0 au format .sb3 directement interprétable informatiquement.



