# Nodered

## How to use

First, install dependencies with npm:

``
npm install
``

Then, you can use it with this command:

``
npm run start
``

Follow instruction from shell to finish, normally, the address is http://127.0.0.1:1880

## How to add package

Open the `package.json` file and add your dependencie or with npm:

``
npm install package
``

See npm [documentation](https://docs.npmjs.com/) for more information

## How to push on quay.io

You need to rebuild a new image with the new dependencies:

``
docker build -t quay.io/suezenv/node-red:latest .
``

Then, push it to quay.io, without forgotten to log on quay.io:

``
docker login quay.io
docker push quay.io/suezenv/node-red:latest
``

## Troubleshoot

**Important**: You need to have an account on quay.io

**Important**: You need to have an access right on suezenv repository, contact your manager for this part.
