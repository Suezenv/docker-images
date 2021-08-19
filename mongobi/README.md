# MongoBI Connector

This image is built based on [jbouzekri/docker-superset-mongo-poc](https://github.com/jbouzekri/docker-superset-mongo-poc/tree/main/mongo-bi)

How to build :

```shell
git clone https://github.com/jbouzekri/docker-superset-mongo-poc
cd docker-superset-mongo-poc/mongo-bi
docker build -t 3slab/mongobi:v2.14.3 .
docker push 3slab/mongobi:v2.14.3
cd ../..
rm -rf docker-superset-mongo-poc
```

*Note : look at current version of mongobi in the dockerfile to correctly tag the image*