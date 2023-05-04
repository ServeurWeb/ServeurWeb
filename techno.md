
# Nos Technologies


## Apache

Pour le serveur web, la start-up a choisi d'utiliser Apache en raison de sa popularité, de sa fiabilité et de sa flexibilité. Apache devra être configuré pour servir les pages web et les applications développées par l'équipe d'Ynnov'Solutions. Il faudra également gérer les certificats SSL pour assurer la sécurité des communications entre le serveur et les clients.


## Reverse proxy avec NGINX

Afin d'améliorer les performances et la sécurité du serveur web, la start-up souhaite mettre en place un reverse proxy avec NGINX. Le reverse proxy sera chargé de répartir les requêtes entrantes entre plusieurs instances d'Apache et de gérer les connexions SSL. NGINX devra également être configuré pour servir les fichiers statiques (images, CSS, JavaScript) et mettre en cache les pages web pour réduire la charge sur le serveur Apache.


## Load balancing avec NGINX

Pour assurer la haute disponibilité du serveur et répartir la charge entre plusieurs serveurs, Ynnov'Solutions souhaite utiliser NGINX pour le load balancing. La configuration de NGINX doit permettre l'ajout et la suppression facile de serveurs en fonction des besoins de l'entreprise. Le load balancing devra également prendre en compte la santé des serveurs et rediriger les requêtes vers les serveurs les moins chargés.



