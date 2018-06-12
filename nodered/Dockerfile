FROM mhart/alpine-node:8.9.4

RUN apk update && \
    apk add git

RUN mkdir -p /usr/src/node-red
RUN mkdir /data

COPY package.json /usr/src/node-red/
WORKDIR /usr/src/node-red

# Install nodered
RUN npm install -g --production
EXPOSE 1880

# Environment variable holding file path for flows configuration
ENV FLOWS=flows.json
ENV NODE_PATH=/usr/src/node-red/node_modules:/data/node_modules

CMD ["npm", "start", "--", "--userDir", "/data"]
