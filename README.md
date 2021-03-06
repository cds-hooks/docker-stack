# what is CDS Hooks?

CDS Hooks provides a pattern for invoking decision support from within a clinician’s EHR workflow.

 * Docs: [cds-hooks.org](http://cds-hooks.org/)
 * Demo: [demo.cds-hooks.org](http://demo.cds-hooks.org/)
 
# use and deploy this stack

## clone this repo with submodules
 * `git clone --recursive https://github.com/cds-hooks/docker-stack`

## update submodules  
 * `git submodule update --init --recursive`

## reference-stack-docker

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
