<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" /></a>
</p>

## Correr Aplicacion

### API GATEWAY

```bash
# * la version de la API es v2 ej: http://localhost:3000/v2/auth/signup

```

```bash

cd api-gateway

npm install

# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

### Microservicio Usuarios

```bash

cd microservice-users

npm install

# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

### Microservicio Restaurante

```bash

cd microservice-restaurants

npm install

# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Despligue con Docker

```bash
# development
# * Tomar en cuenta que cada proyecto se debe haber corrido npm run build para que exista la carpeta /dist
# * Docker se desplegara en el puerto 80
# * la version de la API es v2 ej: http://localhost/v2/auth/signup
docker-compose -f docker-compose.dev.yml up --build -d
```

### Adicional

Se creó una tarea que se ejecuta todos los dias a las 9 am para que los usuario del día anterior  se limpien del restaurante y se comiencen un nuevo dia de atención al cliente.