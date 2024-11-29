# Local Sourcegraph with Docker Compose

> This will be more useful when we can deploy our own Cody instances...

```bash
git checkout release
cd docker-compose
docker compose up -d
# Visit localhost:8888
```

To tear down:
```bash
cd docker-compose
docker compose down
# Nuke databases ...etc
docker volume rm $(docker volume ls -q --filter dangling=true)
```
