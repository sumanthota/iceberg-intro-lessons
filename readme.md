# Directions

To start up the different containers individually.

spark 3.3 with jupyter notebook

```
docker-compose up notebook
```
Access the notebook at http://127.0.0.1:8888. Provide the token from the output 

minio (s3-compatible storage layer)
```
docker-compose up minio
```
Access Minio console at http://127.0.0.1:9001/login

nessie (transactional catalog for Apache Iceberg)

```
docker-compose up nessie
```
Access nessie at http://0.0.0.0:19120/tree/main  

Dremio (data lakehouse platform (query engine, access layer, more))
```
docker-compose up dremio
```
Access dremio at http://localhost:9047/ 

There are three folders in this repo mapped specifically to the spark/notebook container which are:

- `datasets` use this for any sample datasets
- `notebooks` for storing notebooks
- `warehouse` to be used as a warehouse for written data

[Find Guides and Tutorials Here](https://github.com/developer-advocacy-dremio/quick-guides-from-dremio)
