+++
date = "2016-12-20T08:15:34+01:00"
title = "Le Centre Spatial de Kerbin"
url = "centre-spatial"
draft = false

+++

## Présentation du projet

Ce site présente une partie de Kerbal Space Program axée sur un gameplay avancé, semi-réaliste, basé sur l'automatisation. Cette automatisation est rendue possible par l'utilisation du mod [kRPC](http://krpc.github.io/krpc), qui permet d'écrire des programmes de contrôle pour les vaisseaux du jeu en utilisant un langage de programmation réel (j'utilise Python).

Les autres mods utilisés seront décris plus bas.


## Mode de fonctionnement

L'objectif de cette partie de simuler une progression technologique réaliste d'un programme spatial débutant. De plus, il s'agit de concevoir et de lancer des fusées de manière également réaliste; ce qui implique de réutiliser autant que possible les conceptions existantes ou de les faire évoluer, plutôt que de partir d'une feuille blanche pour chaque nouveau besoin (car le développement d'un nouveau matériel prend du temps). Cela implique aussi d'effectuer des lancements d'une manière proche du réel, donc en s'appuyant sur des programmes informatiques de guidage, car même lors d'un vol habité, aucun humain n'a jamais "piloté" le lancement de sa fusée ! Les règles sont donc les suivantes :

* Tout vol, habité ou non, sera automatisé du sol à l'orbite.
* Tout pilotage effectué par un Kerbal sera fait intégralement en vue intérieure (IVA).
* Tout pilotage effectué par une sonde sera fait par un programme. Aucun contrôle direct de la fusée ne sera utilisé.

Le temps nécessaire à l'assemblage d'une fusée sera simulé au travers d'un planning de lancement prenant en compte la complexité du matériel à assembler pour le lancement.


## Mods utilisés

Outre le mod [kRPC](http://krpc.github.io/krpc) déjà cité, voici les mods utilisés pour cette partie qui ont un impact sur le gameplay :

### [USI Life Support](http://forum.kerbalspaceprogram.com/index.php?/topic/105202-12-usi-life-support-050/)

Les vols habités devront être ravitaillés en _Supplies_ et en électricité pour assurer le support vital des kerbals. Ce mod ayant des options plus ou moins strictes, celles-ci seront réglées au plus dur. Un kerbal qui n'a rien à manger pendant plusieurs jours est un kerbal mort !

### [Remote Tech](http://forum.kerbalspaceprogram.com/index.php?/topic/75245-11-remotetech-v1610-2016-04-12/)

Toute communication avec un vaisseau devra être supportée par un réseau de communication actif, fourni par Remote Tech.

### [KScale64](http://forum.kerbalspaceprogram.com/index.php?/topic/87284-kscale64-v1301-ksp-11x-22nd-may-2016/)

Ce mod multiplie par 6,4 les dimensions du système stellaire de Kerbol, afin de se rapprocher des dimensions de notre propre système solaire. Certains paramètres de Kerbin elle-même sont ajustés afin de fournir la meilleure expérience possible :

* période de rotation de 24h
* ligne de Kármán à 93 km (on s'approche des 100 km terriens)
* delta V moyen pour une mise en orbite : 8500 m/s

L'une des principales conséquences de l'utilisation de ce mod (et la raison pour laquelle j'ai décidé de l'utiliser) est que les fusées sont bien plus grandes et plus élancées que celles que l'on construit habituellement dans KSP, ce qui les rend plus réalistes.