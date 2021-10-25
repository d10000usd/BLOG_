# BLOG_



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

# 실행순서

docker --version 

cd frontend && sudo docker run -it node

docker images

docker ps

docker ps -a

https://www.yalco.kr/36_docker/



런할때 필요한 라이브러리 받기

sudo docker run -it node

docker exec -it vibrant_hodgkin bash


# 기본명령어

모든 컨테이너 삭제명령어
docker stop $(docker ps -aq)
docker system prune -a



docker build -t frontend-img .
