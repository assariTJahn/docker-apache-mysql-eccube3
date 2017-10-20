# docker-apache-mysql-eccube3

|      | Version |
|------|---------|
|APACHE| 2.4     |
|PHP   | 7.1     |
|ECCUBE| 3.0     |

## Instruction
1. GIT 이미지 클론 및 디렉토리 생성
```
git clone git@github.com:assariTJahn/docker-apache-mysql-eccube3.git eccube-dev &&\
cd eccube-dev &&\
mkdir db_data
```

2. EC-CUBE3 다운로드 및 압축해제
```
$ wget http://downloads.ec-cube.net/src/eccube-3.0.10.zip
$ unzip eccube-3.0.10.zip
$ ln -s eccube-3.0.10 app
```

3. DOCKER실행
```
$ docker-compose up -d
```

## ETC

ECCUBE3.X GIT리포지터리와 사이트에서 다운가능한 파일의 내용이 다르기 때문에 eccube-3.0.10을 git에서 클론 할 경우 오작동의 가능성이 있음.
