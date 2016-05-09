# reference-stack-docker

To run it, you need Docker >= 1.10, and docker-compose

Edit `docker-compose.override.yml` as needed to configure your preferred local port mappings, then:

 * `docker-compose up`: launch the stack
 * `docker-compose  run tasks load-sample-data`: load sample data


By default, you'll have servers running at ports:

 * `9000`: Test Service
 * `9001`: Inovker

For example, visit http://localhost:9000

---

## Deploy in prod

For example, see [./deploys/cds-hooks.org](./deploys/cds-hooks.org)
