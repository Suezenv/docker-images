# InfluxDB Database Backup

To backup this database, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ cd influxdb
$ docker login docker.io
$ docker build --tag suezenv/phpbu-influxdb:6.0.0-1.7.7 .
$ docker push suezenv/phpbu-influxdb:6.0.0-1.7.7
```
