## Build

```sh
vi .env.production
  VITE_BACKEND_BASE_URL=/api
rm -r dist
./prepare-prod.sh
docker buildx bake --push -f docker-compose.guten.yml 
```