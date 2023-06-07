k6 부하 테스트 툴 (https://k6.io/docs/)
=============
![Alt text](img.png)

사용방법
-------------
---
1. k6 script 실행을 위한 라이브러리 설치 필요
> Max OS   
> >$ brew install k6

> linux (Debian/Ubuntu)
> >$ sudo gpg -k \
> >$ sudo gpg --no-default-keyring --keyring /usr/share/keyrings/k6-archive-keyring.gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C5AD17C747E3415A3642D57D77C6C491D6AC1D69 \
> >$ echo "deb [signed-by=/usr/share/keyrings/k6-archive-keyring.gpg] https://dl.k6.io/deb stable main" | sudo tee /etc/apt/sources.list.d/k6.list \
> >$ sudo apt-get update \
> >$ sudo apt-get install k6 \

2. postman-to-k6 설치 (postman에서 export하는 collections 으로 스크립트 자동생성)
> > $ npm install -g postman-to-k6

3. postman에서 collections.json 파일 export후 스크립트 실행
> > $ k6 run script.js \
> > 참조링크: <https://k6.io/blog/load-testing-with-postman-collections>
