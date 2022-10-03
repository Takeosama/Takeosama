# Activitat 2                                                           Nil Horcas

## Pasos a seguir per fer l'instal·lació 

### 1- Apache
Primerament introduirem la primera comanda per intalar apache2 (sudo apt install apache2) i també (sudo sed -i "s/Options Indexes FollowSymLinks/Options FollowSymLinks/" /etc/apache2/apache2.conf) per desactiva els directoris del servidor.

![capt](apache-1.png)


### 2- Mariadb
Instalarem i configurarem Mariadb amb les seguents comandes: (sudo apt-get install mariadb-server mariadb-client -y) (sudo mysql_secure_installation) (sudo systemctl restart mariadb.service  o  sudo service mariadb.service restart) per reiniciar.

![capt](intallmariadb-2.1.png)    ![capt](mariadb-2.png)

### 3- Base de dades
Entrarem a Mariadb per crea la base de dades on crearem el usuari amb la contrasenya, dona-li acces a la base de dades. Amb les comandes (sudo mysql -u root -p) , (CREATE DATABASE owncloud;) , (CREATE USER 'ownclouduser'@'localhost' IDENTIFIED BY 'Admin1234';) , (GRANT ALL ON owncloud.* TO'ownclouduser'@'localhost' IDENTIFIED BY 'Admin1234' WITH GRANT OPTION;) 


![capt](ownc-3.png)    ![capt](ownc-4.png)
