# Imágenes de Docker sugeridas para los conectores de bases de datos

Asumiendo que tienes instalado [Podman Desktop](https://podman-desktop.io/docs/installation) puedes usar las siguientes imágenes:

## Imagen de MongoDB

`docker.io/mongodb/mongodb-community-server:7.0.8-ubi8`

### Cómo levantar la base de datos MongoDB en un ambiente local

`podman run --name local-mongodb -p 27017:27017 -d mongodb/mongodb-community-server:7.0.8-ubi8`

## Imagen de PostgreSQL

`docker.io/library/postgres:16.2-alpine3.19`

### Cómo levantar la base de datos PostgreSQL en un ambiente local

`podman run --name local-postgres -e POSTGRES_PASSWORD=NoMeLoSe&%$321 -d postgres:16.2-alpine3.19`
