# Casos Prácticos

# Página por defecto:
Para este caso práctico lo único que tendremos que hacer es editar el index.html de inicio de nginx.
la ruta es: /var/www/html/index.html



## Virtual Hosting:
Vamos a crear 2 sitios web, llamados web1 y web2 usando el mismo puerto para eso tendremos que tocar un fichero.

El fichero lo llamaremos web1.conf y web2.conf será una copia editada del archivo default situado en /etc/nginx/sites-avaliable.

Para habilitar el sitio virtual hay que poner el fichero en /etc/nginx/sites-enabled.

![1](./IMAGENES/WEB1.1.png  "WEB1")

![2](./IMAGENES/WEB2.1.png  "WEB2")


## Autenticación,Autorización y control de acceso:

web1 se podra acceder desde la red externa e interna mientras que la web2 solo interna

![3](./IMAGENES/WEB2.SOLO_INTERNA.png "WEB2") 

web1 tendrá un directorio llamado privado que la red interna podrá acceder sin autenticarse mientras que si es por red externa se tendrá que identificar

![4](./IMAGENES/WEB1.AUTHENTICACIÓN.png "WEB1")

## Seguridad

Hacer que el sitio web1 sea seguro hay que decir que antes de eso debemos crear un certificado.

![4](./IMAGENES/WEB1.SSL.png "WEB1")
