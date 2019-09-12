# MongoDB Database Backup

To backup this database, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ cd mongo
$ docker login docker.io
$ docker build --tag suezenv/phpbu-mongodb:5.2.7-4.0.5 .
$ docker push suezenv/phpbu-mongodb:5.2.7-4.0.5
```
