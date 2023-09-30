# Projet 1 : UE8 Architecture de données

## Sommaire :
 -  Description du projet 
 -  La structure du code
 - Le mode d'utilisation
 - Résultats

## 1. Descrition :
L'objectif de ce projet :
Trouver un train et un itinéraire de train depuis la gare choisit en partant de Strasbourg. Cela permet de partir à proximité de la gare, ce qui est souvent un inconvénient des plateformes de randonnées. En effet, les premières randonnées proposées demande souvent l'utilisation d'une voiture.

## 2. Structure : 
Le projet est constitué de 3 parties de code qui sont regroupés en un pour former le projet.
La première, le code donnant tous les trains possibles de la gare de Strasbourg entre deux horaires.
Le deuxième, la partie coordonnée de la ville de la gare choisit
La troisième : le webscraping de l'application komoot qui propose les itinéraires possibles selon les conditions choisit.
La deuxième et la troisième ne fonctionne pas l'une sans l'autre : on a besoin de la ville et des coordonnées pour créer l'url komoot.

## 3. Mode d'utilisation :
Tu choisis la date (J+23 maximum) et les horaires entre lequels tu souhaites partir et on te donne les trains, horaires et destinations possible. Ensuite, tu choisis un trajet parmi ceux proposés, qui permet de trouver des coordonnées GPS (latitude et longitude).  Puis, vient le choix de la durée maximum de la randonnée pour trouver la randonnée idéale. Parfait pour partir au dernier moment.
N.B : Pour les date et les durées, il faut les remplir sous un format particulier pour que cela fonctionne.

## 4.Résultats : 
Le code permet de donner dans la console deux tableaux sous format css. Le premier avec les 40 premiers trajets depuis la gare de Strasbourg avec l'horaire de départ.
Le second avec les radonnées possible par durée décroissante. 
