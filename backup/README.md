# Database Backup

To backup all type of database, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ docker login docker.io
$ docker build --tag suezenv/phpbu:6.0.23 .
$ docker push suezenv/phpbu:6.0.23
```
