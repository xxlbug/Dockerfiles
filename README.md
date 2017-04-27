# Dockerfiles
These files represent some of my docker scripts. I've found examples from other users very useful in learning what you can do with dockerfiles.
*Please enjoy :-)*

# How to use the dockerfiles
* Install docker for your system https://www.docker.com/
## Prism
```
docker run -d -p 4010:4010 -it xxlbug/prism run --validate --list --mock -s /swagger/petstore.swagger
```
## Swagger-UI
```
docker run -p 80:8080 -it xxlbug/swagger-ui
```
