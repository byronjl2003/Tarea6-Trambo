# TAREA 6

## Requerimientos
Para poder ejecutar este ejemplo/Tarea solo necesitan tener instalado docker y docker-compose.

## Acerca del ejemplo/Tarea
La tarea consiste en simular un ambiente de microservicios atraves de docker compose y docker. La arquitectura del sistema consiste en un contenedor que actual como reverse proxy capa 7, que segun la url especificada redirijira la solicitud al servicios correspondiente. Para mas detalle ver la imagen siguiente.

![diagrama][logo]

[logo]:https://raw.githubusercontent.com/byronjl2003/Tarea6-Trambo/master/imagesForREADME/img1.jpeg "diagrama"

## Instrucciones
Colocarse en la carpeta raiz del repositorio y ejecutar el siguiente comando
> $ docker-compose up -d --build

Por ejemplo, para obtener contenido del servidor nginex de contenido estatico ir a http://localhost/static/[nombre del archivo].
* en donde "nombre del archivo es algun archivo que se encuentre en el directorio ./nginx-static/static/" .

Para solicitar la aplicacion de Flask ir a http://localhost/app/

### Descripcion del Repo
* ./flask : Carpeta con el dockerfile para el contendor de la aplicacion flask y los fuentes de la aplicacion

* ./nginx-static : Carpeta con el contenido estatico del nginx de contenido estatico.

* ./nginx-proxy: Carpeta con la configuracion del balanceador de carga.

* ./docker-compose.yml : Archivo con las configuracion para que docker-compose pueda ejecutar nuestra arquitectura.




