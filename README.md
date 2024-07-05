# DataBase_with_docker
database, dockerfile, build commander

## backGound
docker

## commander
이미지 빌드 명령어 (현 파일과 같은 디렉토리에서)
```bash
docker build -t {이미지명} .
```

실행 명령어 (데몬으로 실행)
```bash
docker run --name {컨테이너명} -p 3306:3306 -d {이미지명}
```
