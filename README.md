## Laravel WebSockets Chat Application Example

Realtime chat application built with Laravel WebSockets.

```bash
# Test Database Service
docker-compose ps
docker-compose down
docker-compose up --build
docker-compose ps
docker-compose down
docker-compose ps
mysql -h 127.0.0.1 -P 3307 -u root -p
docker ps -a
docker logs laravel-docker-database-1
docker-compose down

# Test Redis Service
docker-compose up -d
docker-compose ps
redis-cli -h 127.0.0.1 -p 6380
docker ps -a
docker logs laravel-docker-redis-1
docker-compose down
docker-compose ps

# Test PHP Service
chmod +x docker/entrypoint.sh
docker-compose up -d
docker-compose ps
curl 127.0.0.1:8001
docker ps -a
docker logs laravel-docker-php-1
docker exec -it laravel-docker-php-1 bash
docker-compose down

# Test Node Service
docker-compose up -d
docker-compose ps
docker ps -a
docker logs laravel-docker-node-1
docker-compose down

# Test Queue Service
docker-compose up -d
docker-compose ps
docker ps -a
docker logs laravel-docker-queue-1
docker-compose down

# Test Websocket Service
docker-compose up -d
docker-compose ps
docker ps -a
docker logs laravel-docker-websocket-1
# http://127.0.0.1:8001
```