# 100FCProyecto2
## Fundamentos de contenerización
###  Actividad 2.  Modificar un sitio web en ejecución


[Enlace a Docker Hub- Nginx](https://hub.docker.com/_/nginx)

> Paso 1. Partimos de la imagen construida en la actividad anterior, comprobar como se llama:


```
docker image ls
```

> Paso 2. Ejecutar el contenedor en el puerto 8080, con el nombre 100fcproyecto2 y montarel directoiro actual del host
> con el directorio /usr/share/ningx/html dentreo del contenedor.
En Linux,
 ```
docker container run  -d -p 8080:80  --name 100fcproyecto2  -v $(pwd):/usr/share/ningx/html  100fcproyecto1:1.0 
```
en Windows,
 ```
docker container run  -d -p 8080:80  --name 100fcproyecto2  -v %cd%:/usr/share/ningx/html  100fcproyecto1:1.0 
```
Comprobar los contenores en ejecución, y comprobar que sond e la misma imagen:
```
docker ps
```
> Paso 3. Comprobación: http://localhost:8080
> 
> Paso 4. Se pide modificar el fichero index.html desde el contenedor usando el IDE Visual Studio Code
> 

Por último, acceder al navegador http://localhost:8080






