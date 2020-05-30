### Si queres sabes mas sobre mi:
[Nestor Marsollier](https://github.com/nmarsollier/profile)

# Proyecto Mascotas - Programación Avanzada

Proyecto Red social de Mascotas, ejemplo de código para la cátedra "Programación Avanzada" en la Universidad Tecnología Nacional, Facultad Regional Mendoza.

Este proyecto es un ejemplo de como armar un proyecto Node 6 con Typescript como backend, y React como frontend.

El proyecto tiene 2 carpetas

react :  Frontend desarrollado en react y typescript.

node : Node con typescript para backend.

## Guía de Instalación

### Node con npm versión 13+

Seguir la guía de instalación desde el sitio oficial [nodejs.org](https://nodejs.org/)

### MongoDB

Podemos usar docker

```bash
docker run -d --name mascotas-mongo -d -p 27017:27017 mongo:4.0.18-xenial
```

O seguir las guiás de instalación de mongo desde el sitio oficial: [mongodb.com](https://www.mongodb.com/download-center#community)

Sugiero instalar Mongodb Compass para poder navegar la base de datos en forma visual [Compass](https://www.mongodb.com/products/compass)

### Redis

Podemos usar docker

```bash
docker run -d --name mascotas-redis -d -p 6379:6379 redis:5.0.9-buster
```

O seguir los pasos de instalación desde la pagina oficial [redis.io](https://redis.io/download)

Para windows conviene un ejecutable : [Redis Windows](https://sourceforge.net/projects/redis/)

Recomiendo instalar FastoRedis para navegar la base de datos [fastoredis.com](https://fastoredis.com/)

## Ejecución

### Backend

Abrir ventana de comandos en el folder node y ejecutar :

```bash
npm install
npm start
```

El backend expone la documentación de las api abriendo [localhost:3000](http://localhost:3000/)

Pueden ver la documentación del proyecto en [node](./node/README.md)

### React

Abrir ventana de comandos en la carpeta react, ejecutar:

```bash
npm install
npm start
```

Desde un browser debemos abrir [localhost:4200](http://localhost:4200/)

## Docker Producción

Esta instalación y ejecución es muy sencilla, solo pretende permitir la ejecución de todos los contenedores para probarlos.

Una vez levantados los servicios se puede acceder a la app usando [localhost:4200](http://localhost:4200)

Existen 2 yml de compose uno para windows o mac y el otro para linux, hay que bajar y usar el que corresponda desde el repositorio.

Las opciones son las siguientes:

- docker-compose.yml : Para windows y mac, baja y compila todo desde github
- docker-compose-linux.yml : Para linux, baja y compila todo desde github

Levantamos los contenedores usando el comando :

```bash
docker-compose -f docker-XXX.yml up -d
```

## Instalación mas detallada usando solo Docker

No es necesario con compose, pero si queremos algo mas flexible, hay un instructivo :

[Contenedores Docker](READEME-DOCKER.md)
