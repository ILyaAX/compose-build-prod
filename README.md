# compose-build-prod

Using the docker-compose container orchestrator to create 2 services: build and production. The Java application must be created in the build service. 
The application is launched in the productions service. The product image must be of a minimum size.

```
git clone https://github.com/ILyaAX/compose-build-prod.git
```
```
cd compose-build-prod
```
```
docker-compose up -d
```


Product image based on alpine:3.16 - 99.6MB