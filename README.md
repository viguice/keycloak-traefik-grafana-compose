1. Requires [Docker](https://docs.docker.com/engine/install/) with [Compose](https://github.com/docker/compose/releases/latest)
2. Up the project using command `docker compose up -d --wait`

| Command | Discription
|-|-
| `docker stats --no-stream` | Containers resource usage
| `docker compose logs` | Shows logs of containers (use flag `-f` to follow logs)
| `docker compose down` | Stop and remove containers (flag `-v` remove named volumes declared in the volumes section of the Compose file and anonymous volumes attached to containers)
| `docker system prune -a -f` | Remove all unused containers, networks, images (flag `--volumes` prune volumes)

| App | Port | Username | Password | Image
|-|-|-|-|-
| Keycloak | 8080 | `admin` | `keycloak` | ![Keycloak Grafana Client in the realm test](./images/keycloak.jpg)
| Prometheus | 9090 | | | ![Prometheus Targets](./images/prometheus.jpg)
| Grafana | 3000 | `admin` | `grafana` | ![Grafana Keycloak Dashboard](./images/grafana.png)
