# Respuestas

Indica tu nombre a continuación: 

Por cada etapa agrega una sección abajo y escribe las respuestas a las preguntas de cada etapa.

## ETAPA 1

Escribe respuestas de la etapa 1 acá

¿Cuál es la diferencia entre los archivos con el verbo `Create` con los archivos con el verbo `Add`?
R: los Create crean tablas, los Add agregar registros a la tabla

¿Cómo se llama el servicio que se declara en el archivo `docker-compose.yml`?
R: flyway

¿Cuál es el comando que se ejecuta en el servicio declarado?
R:  -locations=filesystem:/flyway/sql -connectRetries=60 migrate

## ETAPA 2
¿Qué pasa si cambias el nombre del servicio de `postgres` a `db`? ¿Qué otros cambios tendrías que hacer?

lab-ic-ms-2023-postgres-1  | 2023-08-08 00:22:59.733 UTC [1] LOG:  database system is ready to accept connections
migration_flyway           | Flyway Community Edition 7.7.0 by Redgate
migration_flyway           | WARNING: Connection error: The connection attempt failed. (Caused by db) Retrying in 1 sec...

R: Da error de conexión. 


## ETAPA 3
### Preguntas

Revisa el archivo `movies-api/Dockerfile`.

¿Qué te llama la atención?
R: es una imagen basada en linux

Revisa el archivo `docker-compose.yml`.

¿Cómo se relacionan el archivo `docker-compose.yml` y el archivo `movies-api/Dockerfile`?
R:  En la declaración de docker-compose es necesario ubicar la ruta donde exista un Dockerfile válido

¿Qué crees que hace el atributo `context` debajo de `build` (está en la linea 6 del archivo `docker-compose.yml`)?
R: Permite definirle a docker-compose la ruta/espacio donde ejecutar una variación a docker build

Recuerda registrar tus respuestas en el archivo `RESPUESTAS.md`


# Etapa 4
Compara los archivos `Dockerfile` de `movies-api` y `movies-front`. 

Compara el atributo `build` del servicio `movies-api` con el de `movies-front`. 

¿Cuál es la diferencia? 

¿Qué pasa si los dejas iguales?