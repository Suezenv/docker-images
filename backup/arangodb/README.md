# arangodb Backup

To backup arangodb, we use [phpbu](http://phpbu.de/).

## Build

To build and release a new version of the image :

*Note : adapt tag version*

```
export PHPBU_VERSION=6.0.5
export ARANGODB_VERSION=3.10.5
docker login docker.io
docker build --build-arg PHPBU_VERSION=${PHPBU_VERSION} --build-arg ARANGODB_VERSION=${ARANGODB_VERSION} --tag suezenv/phpbu-arangodb:${PHPBU_VERSION}-${ARANGODB_VERSION} .
docker push suezenv/phpbu-arangodb:${PHPBU_VERSION}-${ARANGODB_VERSION}
```
