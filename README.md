# Accessibilite-des-langages-de-programmation-par-blocs
Le projet ci-après a pour objectif de rendre accessible par des non-voyants l’utilisation d’un langage de programmation par blocs de type Scratch. Ce projet réalisé au sein de l'IRIT (Institut de Recherche en Informatique de Toulouse) a pour objectif de faciliter l'accès à l'Information par les élèves non voyants.

Ce dispositif comporte des objets tangibles représentant les différents blocs et les différentes variables et un logiciel automatique de reconnaissance de ces objets permettant de générer et d’exécuter le programme conçu par l’utilisateur.

La solution proposée comprend deux aspects.
Il s’agit d’une part de proposer un système permettant la manipulation physique de briques en bois représentant les blocs de base du langage Scratch. Ces pièces, une fois assemblées, forment un algorithme qui est interprété par un ordinateur à l’aide d’outils de reconnaissance visuelle.
Le deuxième enjeu est d’intégrer des outils d’interaction (robots, sorties tactiles ou sonores) rendant l’exécution des algorithmes compréhensibles pour un utilisateur non-voyant. Ce deuxième enjeu n'a pas été complètement implémenté.

Le programme principal du projet (situé sous IntegrationGlobale\src\main\java\Assemblage\CreationScratch.java) prend en entrée un cliché de l'algorithme réalisé physiquement en Scratch (disponible sous ClichesAlgorithmes/Algorithme.jpg) et un fichier ScratchOriginal.zip comprenant la structure d'un programme écrit en Scratch et stocké au format JSON. 
La méthode principale implémente un algorithme de reconnaissance qui transforme un cliché d'un algorithme Scratch en un projet Scratch 3.0 au format .sb3 directement interprétable informatiquement.


Le principe de reconnaissance d'un algorithme Scratch est décrit ci-dessous :
![Reconnaissance Algorithme Scratch](https://user-images.githubusercontent.com/79979599/109825947-9d10bf80-7c3a-11eb-9176-78ce7325e410.PNG)

Dans un second temps le programme va transcrire cet algorithme au format JSON et générer un projet au format .sb3 que l'on pourra importer sous Scratch 3.0 et qui contiendra l'algorithme réalisé.
![Transcription d'un algorithme Scratch](https://user-images.githubusercontent.com/79979599/109826926-959de600-7c3b-11eb-9d77-fc5e38e5ced9.PNG)




