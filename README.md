# containersdemo

## Running Metabase with Docker

To run Metabase in a container, use the following command:

```bash
docker run -d -p 3000:3000 --name metabase metabase/metabase
```

Metabase will be available at [http://localhost:3000](http://localhost:3000).

## Running Uptime Kuma with Docker

To run Uptime Kuma in a container, use the following command:

```bash
docker run -d -p 3001:3001 --name uptime-kuma louislam/uptime-kuma
```

Uptime Kuma will be available at [http://localhost:3001](http://localhost:3001).


## Running PostgreSQL with Docker

To run a PostgreSQL database in a container, use the following command:

```bash
docker run -d \
    --name postgres-db \
    -e POSTGRES_PASSWORD=mysecretpassword \
    -p 5432:5432 \
    postgres
```

Replace `mysecretpassword` with your desired password. PostgreSQL will be available at `localhost:5432`.