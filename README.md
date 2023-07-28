# Projet big data - reconnaissance de fruits sur AWS (pyspark)

Ce dépôt GitHub contient le code source et les ressources nécessaires pour le projet Big Data "Reconnaissance de fruits". L'application développée permet de sélectionner une photo contenant un fruit et de le reconnaître à l'aide d'un modèle de CNN (Convolutional Neural Network) basé sur le transfert learning de MobileNetV2 de Google. Le code est écrit en PySpark et s'exécute sur un cluster AWS EC2 avec un nœud maître et deux nœuds esclaves. De plus, les clés SSH utilisées pour se connecter au serveur se trouvent en Europe pour se conformer au RGPD (Règlement Général sur la Protection des Données).     
II s'agit uniquement de la partie python CNN-L'application n'est pas finit et ce repo ne contient que la partie transfert learning avec spark sur aws.

## Prérequis

1. Un compte AWS permet de créer des instances EC2 et d'accéder à des services connexes.
2. Une paire de clés SSH (clé privée et clé publique) pour se connecter aux instances EC2 en toute sécurité.
3. Un compte S3 pour stocker les données

## Architecture du projet

Le projet est organisé de la manière suivante :
- /data : Ce répertoire contient les données nécessaires pour le projet (images de fruits).
- /notebooks : Ce répertoire contient les notebooks JupyterHub utilisés pour l'exécution du code PySpark.
- /src : Ce répertoire contient le code source du projet, y compris les étapes de prétraitement et le modèle CNN MobileNetV2 pré-entraîné.
- /results : Ce répertoire contient les résultats finaux au format CSV, obtenus à partir de la reconnaissance des fruits.

## Configuration du cluster AWS EC2

Le cluster AWS EC2 est configuré avec les spécifications suivantes :

- Nœud maître : Une instance EC2 avec une configuration adaptée aux besoins de gestion et de coordination du cluster.
- Nœuds esclaves : Deux instances EC2 avec une configuration adaptée au traitement distribué des données.

## Respect de la réglementation RGPD
Les clés SSH utilisées pour accéder au serveur EC2 sont stockées en Europe pour se conformer au RGPD et garantir la protection des données personnelles.

## Conclusion
Nous montrons à travers ce projet les différentes étapes afin de déployer un modèle de machine learning dans le cloud.   

******
Ce projet fait partie de la formation data-scientist de CentraleSupélec & Openclassrooms (certificat bac+5)





