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

## Document

### [EC-CUBE 3.x 개발문서@ec-cube.github.io](http://ec-cube.github.io/)


EC-CUBE 3.x 사양 및 순서、개발팁을 개재하고 있습니다
수정 및 추가기록、신규문서를 만드시는 경우、아래의 리포지터리에 PullRequest를 주십시오.
[https://github.com/EC-CUBE/ec-cube.github.io](https://github.com/EC-CUBE/ec-cube.github.io)

## 開発への参加

EC-CUBE 3.xの不具合の修正、機能のブラッシュアップを目的として、継続的に開発を行っております。  
コードのリファクタリング、不具合修正以外のPullRequestを送る際は、Pull Requestのコメントなどに意図を明確に記載してください。  

Pull Requestの送信前に、Issueにて提議いただく事も可能です。  
Issuesの利用方法については、[こちら](https://github.com/EC-CUBE/ec-cube/wiki/Issues%E3%81%AE%E5%88%A9%E7%94%A8%E6%96%B9%E6%B3%95)をご確認ください。  

[Slack](https://ec-cube.slack.com/messages)でも本体の開発に関する意見交換などを行っております。
