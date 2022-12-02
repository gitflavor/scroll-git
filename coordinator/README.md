# Coordinator

This repo contains the Scroll coordinator.

## Build

```bash
make clean
make coordinator
```

## db config

* db settings in config

```bash
# DB_DSN: db data source name
export DB_DSN="postgres://admin:123456@localhost/test_db?sslmode=disable"
# DB_DRIVER: db driver name
export DB_DRIVER="postgres"
```

## Start

* use default ports and config.json

```bash
./build/bin/coordinator --http
```

* use specified ports and config.json

```bash
./build/bin/coordinator --config ./config.json --http --http.addr localhost --http.port 8390
```