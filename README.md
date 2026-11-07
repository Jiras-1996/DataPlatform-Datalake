# RustFS

Run RustFS independently from this folder with `docker compose up -d`. Copy `.env.example` to `.env` first and set unique credentials. Its persistent object data is stored in the Docker volume `rustfs_data`.

- S3 API: `http://localhost:9000`
- Console: `http://localhost:9001`
- From another container on `data-platform-network`: `http://rustfs:9000`

Create the shared network once before starting either service: `docker network create data-platform-network`.
