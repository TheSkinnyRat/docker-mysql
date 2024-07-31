# GETTING STARTED
## Requirements
- Docker
## How to run this?
1. Go to folder you want to run. For example:
```bash
cd mysql-phpmyadmin
```
2. Run docker compose
```bash
docker compose up -d
```

# FAQ
## How to run multiple version of MySQL?
> [!IMPORTANT]  
> Make sure your mysql version is available in mysql Docker Hub. You can check it [here](https://hub.docker.com/_/mysql).
1. Copy folder and rename
```bash
cp -r mysql-phpmyadmin mysql90-phpmyadmin
```
2. Go to destination folder
```bash
cd mysql90-phpmyadmin
```
3. Change the `.env` file
```env
...
CONTAINER_NAME=mysql-90
MYSQL_VERSION=9.0
...
```
4. Run docker compose
```bash
docker compose up -d
```
