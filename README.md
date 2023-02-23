# Spotify_ETL
La práctica consiste en extraer los datos de varias Playlists en Spotify en formato .json, aplicarle ciertas transformaciones para poder pasar los datos a un formato relacional con forma de estrella. Finalmente, los datos trabajados se cargan a una base de datos, que en este caso, fue Postgres. Mi base de datos fue un contenedor de Docker de Postgres y utilicé un docker-compose para levantar todo lo necesario.

## Requisitos:
- Tener docker instalado, corriendo y un Docker-compose (recomendado ya que hace todo el proceso).
- Instalar las siguientes librerias en Python: pandas, numpy, json, psycopg2, pymysql y sqlalchemy.

## Descripción de Directorios y archivos:
- Carpeta DDLs: contiene los archivos .sql con la estructura de cada tabla y un Jupyter Notebook donde creé las estructuras en la base de datos.
- docker-compose.yml: docker-compose donde levanté la base de datos y definí las formas de conexión.
- ETLs.ipynb: documento Jupyter Notebook donde está todo el desarrollo de la ETL.
- mpd.slice.1000-1999.json: archivo .json con los datos a procesar.

## Estructura Entidad-Relación:
![Image text](https://github.com/dan-behar/Spotify_ETL/blob/main/DDLs/diagramaER.png)