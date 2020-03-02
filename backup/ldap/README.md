# Ldap Backup

To backup ldap, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
$ cd ldap
$ docker login docker.io
$ docker build --tag suezenv/phpbu-ldap:6.0.5-2.4.48 .
$ docker push suezenv/phpbu-ldap:6.0.5-2.4.48
```
