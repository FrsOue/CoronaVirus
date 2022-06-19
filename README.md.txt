
Les Phases de Projet:

 + Data Understanding
 + Data Preparation 
 + Modélisation
 + Power BI Reports
 + Test and Validation 




Objectifs de la partie ETL :
 1 - Extraire les données  a partir du rép covid de l’université John hopkins 
 2 - Nettoyer et transformer les données US confirmed et deaths afin d’avoir la même structure de données globale 
 3 - Supprimer US data du global data qui représente que le total des states
 4 - Faire la concaténation des données US nettoyés avec les données globales 
 5 - Faire un pivoting des colonnes de date pour avoir deux nouveaux colonnes date et valeur contenant tout les dates et leurs valeurs 
   - Convertir le type de la nouvelle colonne date 
 6 - Gérer les valeurs manquantes de la variable province et state en les remplacant par les valeurs  de la variable région 
 7 - Joindre data confirmed et deaths puis les joindre avec Recovery
 8 - Créer 5 nouvelles colonnes pour le calcul des KPI  4
     ( Cas confirmés par jour/ Cas de morts par jour/Cas de  guéris par jour /Taux de mortalité/Taux de guérison )
 9 - Créer la connexion avec SQL server et charger les données transformés dans notre data werehouse  


Processus d’automatisation des données : 

Python : Création d'une fonction contenat les étapes du ETL avec Schedule qui exécute la fonction d’une manière quotidienne,
SQL server : Connexion de la base de données avec python pour charger les nouvelles données transformées 
Power BI : Connexion avec sql server afin d’assurer la mse à jours des dashboards, 


