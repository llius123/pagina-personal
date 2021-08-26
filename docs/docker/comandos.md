---
sidebar_position: 1
---

```docker title="Entorno desarollo"
docker-compose run --service-ports --use-aliases --rm cryptoV1 npm run dev
```

```docker title="Entorno produccion"
docker-compose run --service-ports --use-aliases --rm cryptoV1 rm -f -R dist/
docker-compose run --service-ports --use-aliases --rm cryptoV1 npm run build2
docker-compose run --service-ports --use-aliases --rm cryptoV1 node ./dist/index.js
```
