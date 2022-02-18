# Diplomado en Ciberseguridad - Mod_3.4 Ciberseguridad en la nube e IoT
## Examen Docker

A continuación las instrucciones para desplegar contenedor:

 1. Una vez que tenemos una cuenta creada en Docker Hub, accedemos a dicha plataforma con la siguiente sentencia:
 
```
docker login
```
Nos pedirá el nombre de usuario y la contraseña con la que nos dimos de alta en Docker Hub.


2. Antes de obtener la imagen de Docker Hub, debemos asegurarnos de contar con la página Web de prueba, el archivo index.html correspondiente se debe encontrar en el directorio actual, es decir, en el directorio en el que se ejecutará la sentencia para la ejecución de la imagen.

3. Para obtener la imagen y ejecutarla localmente en nuestro equipo, debemos ejecutar la siguiente sentencia:

```
docker run -dit --name examen-cloud_10 -p 8080:80 -v "$PWD":/usr/local/apache2/htdocs/ jmillanba/examen-docker:1.0
```

Esto levantará el contenedor y el servicio quedará abierto en el puerto 8080.
