# Elasticsearch Database Backup

To backup this database, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ cd elasticsearch
$ docker login docker.io
$ docker build --tag suezenv/phpbu-elastic:5.2.7-6.3.3 .
$ docker push suezenv/phpbu-elastic:5.2.7-6.3.3
```
