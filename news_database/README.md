# DataBase_with_docker
database, dockerfile, build commander

## backGound
docker
## Docker Hub에서 MongoDB 이미지 다운로드 및 실행
```bash
mkdir my-mongo
cd my-mongo

```
## Dockerfile
```bash
FROM mongo:latest
# COPY mongod.conf /etc/mongod.conf
# COPY init-data.js /docker-entrypoint-initdb.d/

#  port settting
EXPOSE 9200
```

## commander
이미지 빌드 명령어 (현 파일과 같은 디렉토리에서)
```bash
docker build -t my-mongo-image .
```

실행 명령어 (데몬으로 실행)
```bash
docker run --name my-mongo-container -d my-mongo-image
```

