# InfluxDB relay

Fork of [AppAccellerator InfluxDB Relay image](https://github.com/appcelerator-archive/docker-influxdb-relay)

https://github.com/influxdata/influxdb-relay

## Run the container

    docker -e HTTP_BACKEND_influxdb_a=influxdb-a:8086 -e HTTP_BACKEND_influxdb_b=influxdb-b:8086 \
           run appcelerator/haproxy-relay

## Configuration

Variable | Description | Default value | Sample value
-------- | ----------- | ------------- | ------------
HTTP_BIND_ADDR | bind address for the HTTP listener | :9096 |
HTTP_BUFFER_SIZE_MB | See [Buffering](https://github.com/influxdata/influxdb-relay#buffering) | 0 |
HTTP_MAX_BATCH_KB | See [Buffering](https://github.com/influxdata/influxdb-relay#buffering) | 512 |
HTTP_MAX_DELAY_INTERVAL | See [Buffering](https://github.com/influxdata/influxdb-relay#buffering) | 10s |
UDP_BIND_ADDR | bind address for the UDP listener | :9096 |
HTTP_BACKEND_xx | host:port of an influxDB backend, http protocol | | influxdb-backend:8086
UDP_BACKEND_xx | host:port of an influxDB backend, udp protocol | | influxdb-backend:8086
UDP_MTU | UDP MTU | 512 | 1024
