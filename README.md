# Traefik in Docker Template

This is a template for running [Traefik](https://traefik.io/) in Docker. It includes a basic setup with Docker Compose and a sample configuration file.

## How to Use

### Create Docker Network

First, create a network for docker containers to communicate with each other. This is necessary for Traefik to route traffic to the correct containers.

```bash
docker network create proxy_router
```

### Start Docker Compose

```bash
docker compose up -d
```

### You can also use the pre-defined script to start the containers:

```bash
./setup.sh
```

For more information, please see [Traefik Documentation](https://doc.traefik.io/traefik/getting-started/quick-start/)
