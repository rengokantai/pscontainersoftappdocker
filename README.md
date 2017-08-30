# pscontainersoftappdocker
## 3. Committing Containers to Images
### 2 Committing a Container to an Image
```
docker image pull memcached
```

```
docker container run alpine apk add --no-cache python
docker container ls -l --format 'table {{.ID}}\t{{.Image}}\t{{.Command}}'
```
we can get container ID 1234567
```
docker container diff 1234567
docker container commit -m "" 1234567 my-image:1.0
docker image ls --format 'table {{.Repository}}{{.Tag}}{{.ID}}{{.Size}}' my-image:1.0
```
