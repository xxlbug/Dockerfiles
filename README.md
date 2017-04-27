# Dockerfiles
These files represent some of my docker scripts. I've found examples from other users very useful in learning what you can do with dockerfiles.

*Please enjoy :-)*

# How to use the dockerfiles

* Install docker for your system https://www.docker.com/

## prism
See https://github.com/stoplightio/prism for more information
```
docker run -d -p 4010:4010 -it xxlbug/prism run --validate --list --mock -s /swagger/petstore.swagger
```

## swagger-ui
See https://github.com/swagger-api/swagger-ui for more information
```
docker run -p 80:8080 -it xxlbug/swagger-ui
```

## swagger-editor
See https://github.com/swagger-api/swagger-editor for more information
```
docker run -p 80:8080 -it xxlbug/swagger-editor
```

## nginx
See https://www.nginx.com/ for more information
```
docker run -it xxlbug/nginx
```

*Attention*: This command starts nginx *without* randomized ports on every start of the container (default ports are 80 and 443).
If you want to randomize the used ports start the container like so
```
docker run -P -it xxlbug/nginx
```

and get the currently used ports with
```
docker ps
```
