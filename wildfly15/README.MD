# Dockerfile for Wildfly 15 
Contains Wildfly 15 with management console enabled.
* User/Pass: admin 

## Build Docker image 
 ```shell
docker build -t wildfly15/davvidk .
```

## Start docker container
```shell
docker run -p 9990:9990 -p 8080:8080 -it wildfly15/davvidk
```

### Start Management console 
```shell
http://localhost:9990/console
```