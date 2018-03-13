FROM mhart/alpine-node:8.9.4

WORKDIR /data
COPY package.json /data

# Install nodered
RUN npm install 
EXPOSE 1880

# Environment variable holding file path for flows configuration
ENV FLOWS=flows.json
ENV NODE_PATH=/usr/lib/node_modules:/data/node_modules

CMD ["node-red"]
