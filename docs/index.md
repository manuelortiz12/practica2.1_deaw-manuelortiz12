# PRACTICA 2.1: Instalación y configuración de un servidor web Nginx

## INSTALACION NGINX
![1](capturas/1.png)

Comprobamos que esté funcionando:

![2](capturas/2.png)

## CREACION DEL DIRECTORIO DEL SITIO WEB

Creamos el directorio y haremos que el propietario de esta carpeta y todo lo que haya dentro sea el usuario www-data, además de proporcionarle los permisos pertinentes.
Además clonamos el siguiente repositorio en este:

![3](capturas/3.png)

Ahora entramos al navegador con nuestra ip y nos sale lo siguiente:

![4](capturas/4.png)

## CONFIGURACION DEL SERVIDOR WEB NGINX

Debemos modificar el siguiente archivo:
```
/etc/nginx/sites-available/vuestro_dominio
```
![5](capturas/5.png)
![6](capturas/6.png)

Primero antes de nada modificaremos el archivo /etc/hosts para que nuestra máquina anfitriona asocie la IP de la máquina virtual con el nombre del servidor

![alt](capturas/7.png)

Y comprobaremos los logs.

## CONFIGURAR SERVIDOR SFTP EN DEBIAN

Primero instalamos vsftpd y creamos una carpeta /ftp en el home de la máquina virtual.

Después creamos los certificados de seguridad necesarios para aportar la capa de cifrado a nuestra conexión.

![8](capturas/8.png)

A continuación realizaremos la configuración de vsftpd

Abrimos el siguiente archivo de configuracion:

![9](capturas/9.png)

Y añadimos lo siguiente:

![10](capturas/10.png)

Y reiniciamos.

## AÑADIR ARCHIVOS MEDIANTE FILEZILLA

Descargamos filezilla en nuestro pc y le ponemos las siguientes especificaciones:

![11](capturas/11.png)

Conectamos y ya podremos transferir archivos con la máquina virtual.