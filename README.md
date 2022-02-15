## Dockerized Nginx

Basic Docker setup to keep me from having to install Nginx directly onto a machine when doing reverse proxies.

## TL;DR
Get the codebase and install dependencies:
```bash
git clone https://github.com/vbhayden/docker-nginx
cd docker-nginx
sudo ./install-reqs.sh
```
Configure your Nginx instance by copying the example environment file and adding your own values:
```
cp example.env .env
```

You'll also need to configure a basic config file for it to use:
```
cp nginx/default.example.conf nginx/default.conf
```

Stand it up:
```
sudo docker-compose up -d --build
```
