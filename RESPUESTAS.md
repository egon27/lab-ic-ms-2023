# Respuestas

Indica tu nombre a continuación: 

Por cada etapa agrega una sección abajo y escribe las respuestas a las preguntas de cada etapa.

## ETAPA 1

Escribe respuestas de la etapa 1 acá

¿Cuál es la diferencia entre los archivos con el verbo `Create` con los archivos con el verbo `Add`?
los Create crean tablas, los Add agregar registros a la tabla

¿Cómo se llama el servicio que se declara en el archivo `docker-compose.yml`?
flyway

¿Cuál es el comando que se ejecuta en el servicio declarado?
-locations=filesystem:/flyway/sql -connectRetries=60 migrate

## ETAPA 2
¿Qué pasa si cambias el nombre del servicio de `postgres` a `db`? ¿Qué otros cambios tendrías que hacer?

lab-ic-ms-2023-postgres-1  | 2023-08-08 00:22:59.733 UTC [1] LOG:  database system is ready to accept connections
migration_flyway           | Flyway Community Edition 7.7.0 by Redgate
migration_flyway           | WARNING: Connection error: The connection attempt failed. (Caused by db) Retrying in 1 sec...

Da error de conexión. 