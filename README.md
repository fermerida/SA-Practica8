# Practica 8 SA

En esta practica se utilizaran dos contenedores en Docker Compose que involucren:
Un servidor web
Una base de datos 

Esto con la finalidad de implementar la utilización de contenedores como herramienta de construcción de un entorno. 

## Demostración

Video de la demostración de la practica 8:
[Video](https://youtu.be/0BUWUHwjf5k)



## Getting Started

Para correr la practica será necesario acceder a su carpeta y correr el siguiente comando en la terminal.
```
node app.js
```
Esto mostrará el inicio y se podrá seleccionar una de las funcionalidades especificadas previamente. 

Se tienen dos carpetas distribuidas de la siguiente manera:

### Comandos

Repositorio base de datos ----> docker pull 201314713/s1p1-db

Repositorio Api ----> docker pull 201314713/s1p1-api

Repositorio Web ----> docker pull 201314713/s1p1-web

### Compose:
docker-compose.yml: crea y alista el entorno de trabajo total creando todas las imagenes necesarias para correr la pagina web (En el puerto 3258) utilizar con comando docker-compose up

### DB:

-Dockerfile: recursos para la base de datos, el DockerFile genera una base de datos MYSQL corriendo en el puerto 3306

-mysql-scripts: carpeta con los scripts de la base de datos, se tienen dos uno de creación de tablas, en este caso producto, y una de llenado de tablas con datos predeterminados.

### API:

-Dockerfile: recursos para la generación de la api y del servidor web

-views: paginas para el servidor web

-app.js: appi de NodeJS utilizando un servicio de REST api en el puerto 3258

### WEB:

	-Servidor NGINX en el puerto 80 actuando para los datos de la API ubicada en el puerto 3258
	- Su configuración se encuentra en el Docker-compose.yml en odnde descarga los recursos necesarios para su utilización y configura las carpetas de la misma para que reciba toda la información de NODEJS


### Prerequisitos

Esta aplicación sera implementada utilizando JavaScript y Docker. Para su utilización sera necesario tener
* **NodeJS**
* **Docker**

### Instalación de dependencias

Para instalar todas las dependencias es necesario utilizar el siguiente comando
```
npm install
```

### Construido con

* **NodeJS** - El framework de desarrollo
* **Express** - Utilizado un servidor mediante la utilización de express para que pueda consumir la API externa
* **Javascript** - Lenguaje de desarrollo
* **Html** - Para la visualización de las opciones

# Formateo y estandarés de codigo

Al utilizarse Javascript para la implementación se selecciono el estandard de codigo [Standard JS](https://standardjs.com/)

Tambien se utilizo html con el estandard de codigo [Ckan](https://docs.ckan.org/en/2.8/contributing/html.html)

# Author

Author de la practica como parte del curso de Software avanzado de la Universidad de San Carlos de Guatemala.

Fernando Andrés Mérida Antón - 201314713