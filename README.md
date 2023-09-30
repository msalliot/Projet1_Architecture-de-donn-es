# Projet 1 : UE8 Architecture de données

## Sommaire :
 - Description du projet 
 - La structure
 - Description des parties du code
 - Le mode d'utilisation
 - Résultats

## 1. Descrition :
L'objectif de ce projet :
Trouver un train et un itinéraire de train depuis la gare choisit en partant de Strasbourg. Cela permet de partir à proximité de la gare, ce qui est souvent un inconvénient des plateformes de randonnées. En effet, les premières randonnées proposées demande souvent l'utilisation d'une voiture.

## 2. Structure : 
- Readme : explications concises du projet
- Codeentier_rando.ipynb : codes sous format jupyter notebook du projet

# 3. Description des parties du code :  
Le projet est constitué de 3 parties de code qui sont regroupés en un pour former le projet.  
La première :  le code donne tous les trains possibles de la gare de Strasbourg entre deux horaires. Pour se faire, nous utilisons l'API de la sncf : "https://numerique.sncf.com/startup/api/token-developpeur/"  
La deuxième : la partie concerne les coordonnées de la ville de la gare choisit. L'API de "https://geo.api.gouv.fr/communes" est utilisé.  
La troisième : Elle concerne le webscraping de l'application komoot qui propose les itinéraires possibles selon les conditions choisies. La deuxième et la troisième parties ne fonctionnent pas l'une sans l'autre : on a besoin de la ville et des coordonnées pour créer l'url komoot.

## 4. Mode d'utilisation :
Tu choisis la date (J+23 maximum) et les horaires entre lequels tu souhaites partir et on te donne les trains, horaires et destinations possible. Ensuite, tu choisis un trajet parmi ceux proposés, qui permet de trouver des coordonnées GPS (latitude et longitude).  Puis, vient le choix de la durée maximum de la randonnée pour trouver la randonnée idéale. Parfait pour partir au dernier moment.  
N.B : Pour les date et les durées, il faut les remplir sous un format particulier pour que cela fonctionne.

## 5. Résultats : 
Le code permet de donner dans la console deux tableaux sous format css. Le premier avec les 40 premiers trajets depuis la gare de Strasbourg avec l'horaire de départ. Le second avec les randonnées possibles par durée décroissante. 
