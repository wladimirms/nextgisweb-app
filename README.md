# nextgisweb_image

## build docker image

```bash
docker build -t tsnigri/nextgisweb:latest .
```

## run container

```
docker run -d -p 8080:8080 --name nextgisweb-app tsnigri/nextgisweb:dev
```

## run in interactive mode

```
docker container run -it --publish 8080:8080 tsnigri/nextgisweb:dev //nextgisweb initialize_db && uwsgi --ini uwsgi.ini
```

## start container

```
docker container start nextgisweb-app 
```

## stop container

```
docker container stop nextgisweb-app 
```

## remove container

```
docker container rm nextgisweb-app 
```