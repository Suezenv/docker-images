# PostgreSQL Database Backup

To backup this database, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ cd postgresql
$ docker login docker.io
$ docker build --tag suezenv/phpbu-postgresql:6.0.14-11.10 .
$ docker push suezenv/phpbu-postgresql:6.0.14-11.10
```
