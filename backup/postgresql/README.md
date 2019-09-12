# PostgreSQL Database Backup

To backup this database, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ cd postgresql
$ docker login docker.io
$ docker build --tag suezenv/phpbu-postgresql:5.2.7-11.4 .
$ docker push suezenv/phpbu-postgresql:5.2.7-11.4
```
