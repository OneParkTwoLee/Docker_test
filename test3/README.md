# Docker_test
## 3. test3

**Dockerfile**
fastai 등의 라이브러리를 사용하기 위해 파이썬 버전을 3.6으로 설정했다.

**requirements.txt**
api.py 파일에서 사용하며 pip3로 설치하기 위해 필요한 라이브러리 이름들을 모아놓은 파일.

- PIL은 pillow로 대신 설치

- time,io는 파이썬에 이미 내장되어 있고 fastai.vision도 fastai에 포함되어 있어 따로 설치x
+)추후 최종에서 테스트 한 결과 Flask, flask_restful, aiohttp, fastai만 설치하면 된다.

**api.py, picture.py, status.py**
dockerfile에서 api.py 파일 실행. 해당 organization의  PracticeFlaskRESTful/model_inference_restful 폴더 파일과 동일.api.py만 일부 수정

**명령어**
```
$docker build --no-cache -t flask-restful_rerere:latest .
$ docker run -d -p 5000:5000 flask-restful_rerere
```

> test1, test2와 달리 설치해야될 라이브러리 때문에 파이썬의 버전을 3.6으로 설정했다. 해당 버전의 파이썬을 다운 받기 위해 다커 이미지를 생성할 때 `--no-cahe`를 추가해 주었다



* ### 결과 화면 
안드로이드의 에뮬레이터에 사자 사진을 저장하고 해당 사진을 플라스크 서버로 보내면 화면에 lion이라고 뜬다. 해당 안드로이드 프로젝트는 psystar99/Docker_test 리포지토리에 있다.
![스크린샷 2020-08-09 오후 10 41 48](https://user-images.githubusercontent.com/40908279/89733606-841fa180-da91-11ea-86da-26828764c437.png)

안드로이드 코드: https://github.com/Psystar99/Docker_test
* * *
