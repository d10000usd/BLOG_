# BLOG_upload

GIT

echo "# BLOG_" >> README.md

git init

git add README.md

git add -A

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/d10000usd/BLOG_.git

git push -u origin main

git status

# Docker 받고 프레임 실행순서

docker --version

cd frontend && sudo docker run -it node

docker-compose up -d

docker images

docker ps

docker ps -a

## 참고 https://www.yalco.kr/36_docker/

런할때 필요한 라이브러리 받기

sudo docker run -it node

docker exec -it vibrant_hodgkin bash

# 기본명령어

모든 컨테이너 삭제명령어
docker stop $(docker ps -aq)
docker system prune -a

docker build -t frontend-img .

docker build -t database-img
docker run --name database-con -p 3306:3306 -d database-img
docker logs -f database-con

# 파이썬 관련 설치

pip install flask-mysql
pip install -U flask-cors
conda install -c conda-forge mysql-client

# Git


> git init      <=== 깃 폴더 이동후 깃사용 초기화
> git config user.name  <=== 유저내임확인  git config user.name "d10000usd" 초기화가능
> git config user.email <=== 유저이메일  git config user.name "d10000usd@gmail.com" 초기화가능, 12~@!@!

git에다 저장소 만들고

> 셋팅방법
> echo "# REPO" >> README.md
> git init
> git add README.md
> git commit -m "first commit"
> git branch -M main
> git remote add origin https://github.com/d10000usd/REPO.git
> git push -u origin main

git full





명령어

> git status
> touch h.html
> git add -A       <=== 변경확인 및 캡슐화
> git status      <===깃상태 확인
> git commit -m "com1"        <===커및이름을 포함해서 커밋
> git push        <=== 깃허브에 업로드

git log

> -->> 앞에 6자리
> commit d89380571e603d8e78b6c0fbcb34e8503abe4a63 (HEAD -> main)
> Author: HG <d10000usd@gmail.com>
> Date:   Fri Oct 22 23:49:53 2021 +0900

> git reset d89380 --hard
> --> 작업한걸 기준으로 다지우고 새로 시작, 기준점 이후작업한걸 다시 찾지는 못함

> git revert d89380
> --> 기준점 으로 이동하하나 로그가 남아있어서, 기준점 이후 작업으로도 갈 수가 있다.

> git checkout -b my-idea-2
> git branch -D my-idea       <===브랜치삭제
> git branch my-idea  <=== 브랜치 생성
> git branch -a
> git checkout my-idea <=== my-idea 브랜치로 이동
> git fetch

> git checkout main   <=== main 브랜치로 이동
> git merge my-idea       <=== vim 에서 wq 해주면 적용 완료
> -->적용

> git rease my-idea
> git log --graph --all --decorate

> git remote      <=== 리모트 이름

> .gitignore      <=== 없으면 만들고, 이씅면 여기 안에다가 숨겨야할 파일을 넣어두면 깃에 없로드가 되지 않음

> git fetch       <===깃허브에 정보를 가져오고
> git branch -a   <===브랜치 이름들을 가져온후
> git checkout -b my-idea origin/my-idea-2        <=== my-idea 체크아웃, 깃허브 푸쉬명오리진/브랜치이름 origin/my-idea-2

> git push -d origin my-idea-2        <===깃허브 브랜치 삭제 방법

> 깃허브 키체인 설정
> https://architectophile.tistory.com/13
> https://www.yalco.kr/_02_github_token/
> keychain access
> github.com 에서 해슁된 패스워드 삽입
> push 할때 팝업이 나오는건 기본 파일 권한 암호와 동일하게 설정 :: hghg
> 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
