# Servidor NGINX


## ¿Que es NGINX?
Es un servidor web/proxy inverso ligero de alto rendimiento y un proxy para protocolos de correo electrónico.Es software libre y de código abierto, licenciado bajo la Licencia BSD simplificada; también existe una versión comercial distribuida bajo el nombre de Nginx Plus.


## ¿Que se diferencia con apache?
La diferencia con apache es que nginx tiene un mejor soporte de usuarios gracias a sus gestión de procesos.


## Esquema
El esquema de red que utilizaremos será el siguiente:


![Red](/IMAGENES/Red.png "Red")



## Instalación
Para instalar NGINX lo único que tendremos que hacer es un *apt install nginx* y nos instalará nuestro servidor NGINX.

## Casos Prácticos
Página por defecto:
Para este caso práctico lo único que tendremos que hacer es editar el index.html de inicio de nginx.
cd /var/www/html/index.html



Virtual Hosting:
Vamos a crear 2 sitios web, llamados web1 y web2 usando el mismo puerto para eso tendremos que tocar un fichero.

El fichero lo llamaremos web1.conf y web2.conf.

![1](/IMAGENES/WEB1.1.png  "WEB1")

![2](/IMAGENES/WEB2.1.png  "WEB2")


Autenticación,Autorización y control de acceso

web1 se podra acceder desde la red externa e interna mientras que la web2 solo interna

![3](/IMAGENES/WEB2.SOLO INTERNA.png "WEB2) 

## Referencias
