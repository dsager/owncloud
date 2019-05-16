# owncloud
owncloud docker environment

## local setup

Clone the repo
```
git clone git@github.com:dsager/owncloud.git
```

Create `.env` file with following content
```
OWNCLOUD_VERSION=10.0
OWNCLOUD_DOMAIN=localhost
ADMIN_USERNAME=admin
ADMIN_PASSWORD=admin
HTTP_PORT=80
```

Start containers `owncloud`, `db` & `redis`
```
docker-compose up -d
docker-compose ps
```

Run bash shell in container
```
docker-compose exec owncloud bash
```
