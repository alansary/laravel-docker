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

# Test Redis Service
docker-compose up -d
docker-compose ps
redis-cli -h 127.0.0.1 -p 6380
docker-compose down
docker-compose ps

# Test PHP Service
chmod +x docker/entrypoint.sh
docker-compose up -d
docker-compose ps
curl 127.0.0.1:8001
docker-compose down
```