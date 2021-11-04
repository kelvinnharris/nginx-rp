# Task A1

Run a reverse proxy with NGINX,

## Steps to reproduce

Run the following command. This will create the containers and run them from configuration in `docker-compose.yml`.

```
$ docker-compose up
```

In `docker-compose.yml` line 5, it builds an image based on `Dockerfile` in current directory. This `Dockerfile` creates a simple NGINX reverse proxy based on `nginx.conf` file.

To access the proxied servers (which is also a NGINX application), go to

```
http://localhost:80/
```

The following diagram illustrates how the reverse proxy proxies the servers.

![](diagram.jpg)

