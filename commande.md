[Sommaire](./README.md)



# Création du serveur web

## Installer serveur Apache 
sudo apt-get install apache2

## Création du fichier pour ajouter notre site web
sudo mkdir /var/www/monsite


## Donne les permissions
sudo chown -R www-data:www-data /var/www/monsite


## Créer un fichier conf pour pouvoir configurer notre virtual host
sudo nano /etc/apache2/sites-available/monsite.conf


## Ajouter ce code à l'intérieur
<VirtualHost *:80> ServerName monsite.com ServerAlias www.monsite.com DocumentRoot /var/www/monsite ErrorLog ${APACHE_LOG_DIR}/error.log CustomLog ${APACHE_LOG_DIR}/access.log combined </VirtualHost> 


## Exécuter le code 
sudo a2ensite monsite.conf


## Redémarrer Apache
sudo systemctl restart apache2


## Lancer le serveur Apache
sudo systemctl start apache2


## Arreter le serveur
sudo systemctl stop apache2


## Lancer automatiquement au démarrage de la vm
sudo systemctl enable apache2


## Etat du serveur
sudo systemctl status apache2


## Installer Php
sudo apt-get install libapache2-mod-php


## Lancer Sql
sudo systemctl start mysql


## Etat sql
sudo systemctl status mysql


## Regarder sur internet si notre serveur marche
Mettre notre adresse Ip (ex: http://192.168.??.??/)


## Trouver son Ip
ip addr show


## Installer Python3
sudo apt-get install python3

Ces étapes vous permettront de créer et de configurer un serveur web Apache avec PHP et Python sur votre machine virtuelle. Assurez-vous de suivre les instructions avec précision pour garantir le bon fonctionnement de votre serveur web.