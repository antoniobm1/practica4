# practica4
La url del repositorio de la practica 4 es el siguiente:
      https://github.com/antoniobm1/practica4.git
      
## Instalacion segundo Apache
Entramos en Amazon y creamos una instancia, la cual vamos a instalar un Apache.

Este Apache va a ser el 2 front-end, utilizamos las mismas maquinas de la practica 3 y aqui en la 4 añadimos 1 front-end mas.

Lo vamos a instalar igual que en la 3 con el siguiente script.

```
#!/bin/bash
#Imprime las líneas de entrada con las expansiones realizadas, es decir, tal como serán ejecutada
set -x

#Actualizamos los repositorios
sudo apt-get update

#Instalamos apache
sudo apt-get install apache2 -y

#Instalamos paquetes para apache
sudo apt-get install php libapache2-mod-php php-mysql -y

#Instalamos adminer
cd /var/www/html
mkdir adminer
cd adminer
sudo wget https://github.com/vrana/adminer/releases/download/v4.3.1/adminer-4.3.1-mysq$
sudo mv adminer-4.3.1-mysql.php index.php
´´´
