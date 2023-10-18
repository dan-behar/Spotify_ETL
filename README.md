# Spotify_ETL
The practice involves extracting data from various Spotify playlists in .json format and applying certain transformations to convert the data into a star-shaped relational format. Finally, the processed data is loaded into a database, in this case, using Postgres. My database was a Postgres Docker container, and I used a docker-compose to set up everything that was needed.

## Requirements:
- Have Docker running and a docker-compose file.
- Install the following Python libraries: pandas, numpy, json, psycopg2, pymysql y sqlalchemy.

## Directories and Files:
- Carpeta DDLs: holds the .sql files with each table structure and a Jupyter notebook in which I created those structures in the Database.
- docker-compose.yml: docker-compose to build the database and the connections.
- ETLs.ipynb: jupyter notebook with the creation of the ETL.
- mpd.slice.1000-1999.json: .json file with the raw data.

## Diagram of the Database:
![Image text](https://github.com/dan-behar/Spotify_ETL/blob/main/DDLs/diagramaER.png)
