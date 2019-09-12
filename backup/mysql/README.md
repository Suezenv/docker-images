# MySQL Database Backup

To backup this database, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ cd mysql
$ docker login docker.io
$ docker build --tag suezenv/phpbu-mysql:5.2.7-10.3.16 .
$ docker push suezenv/phpbu-mysql:5.2.7-10.3.16
```
