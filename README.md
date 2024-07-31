# GETTING STARTED
## Requirements
- Docker
## How to run this?
1. Go to folder you want to run. For example:
```bash
cd mariadb-phpmyadmin
```
2. Run docker compose
```bash
docker compose up -d
```

# FAQ
## How to run multiple version of MariaDB?
> [!IMPORTANT]  
> Make sure your mariadb version is available in MariaDB Docker Hub. You can check it [here](https://hub.docker.com/_/mariadb).
1. Copy folder and rename
```bash
cp -r mariadb-phpmyadmin mariadb110-phpmyadmin
```
2. Go to destination folder
```bash
cd mariadb110-phpmyadmin
```
3. Change the `.env` file
```env
...
CONTAINER_NAME=mariadb-110
MARIADB_VERSION=11.0
...
```
4. Run docker compose
```bash
docker compose up -d
```
