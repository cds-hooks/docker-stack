## Deploy to demo.syncfor.science


### Prepare the remote docker-machine

```
eval $(docker-machine env demo-host)
docker network create nginx-proxy
```

### Launch the stack

```
docker-compose \
  -f docker-compose.yml \
  -f deploys/cds-hooks.org/docker-compose.yml \
  up -d
```
