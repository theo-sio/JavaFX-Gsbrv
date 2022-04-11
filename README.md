# JavaFX-Gsbrv
GSB Rapports Visite - module Délégué Régional – par @Aaldn

Java 17 JavaFX 17 Gradle 7 Mariadb 10

Application de bureau de suivi des rapports de visite.

 
 
Documentation
Documentation utilisateur
Documentation technique
Contexte
GSB - Fiche descriptive
GSB - Cas d'utilisation
GSB - Modèle Entité-Association
GSB - Cahier des charges
Prérequis
Java 17 + définition de la variable d'environnement JAVA_HOME
MariaDB
En cas de difficulté, reportez-vous à la documentation officielle de JavaFX et de MariaDB.

Installation
Tout d'abord, clonez ce dépôt puis placez-vous au sein du projet :

$ git clone https://github.com/Aaldn/GSB-RV-DR
$ cd GSB-RV-DR
Ensuite, exécutez le script de création de la base de données et créez son utilisateur :

$ mariadb -e "source sql/gsb_rv.sql;"
$ mariadb -e "grant all privileges on gsb_rv.* to developpeur identified by \"azerty\";"
Enfin, lancez l'application :

$ ./gradlew run
Licence
Voir le fichier LICENSE.md fourni.
