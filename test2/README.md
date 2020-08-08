# Docker_test
## 2. test2

Dockerfile, app.py, requirements.txt 생성 후 명령어실행

 
**명령어**
```
$ docker build -t flask-application_second_rerere:latest .
$ docker run -d -p 5000:5000 flask-application_second_rerere
```

* ### 결과 화면 
http://127.0.0.1:5000/plus?x=2&y=3 주소를 웹 브라우저에 치면 {"result": 5}가 뜬다
<img width="557" alt="test2" src="https://user-images.githubusercontent.com/40908279/89118360-21059c00-d4e0-11ea-8dac-f37e0f349d05.png">

참고 https://m.blog.naver.com/PostView.nhn?blogId=wideeyed&logNo=221350669178&proxyReferer=https:%2F%2Fwww.google.com%2F
* * *

해당 url과 안드로이드 에뮬러이터와의 통신 by okhttp3. 이때 url을 127.0.0.1로 설정하면 에뮬레어터가 자신이라 생각하기에 에러가 난다. 로컬호스트 이름이 아닌 ip주소를 사용한다.
> 브라우저
<img width="474" alt="스크린샷 2020-08-08 오전 10 54 53" src="https://user-images.githubusercontent.com/40908279/89699936-a74d3280-d965-11ea-8dc9-d16d4eeb96d7.png">

> 안드로이드 에뮬레이터
<img width="342" alt="스크린샷 2020-08-08 오전 10 48 49" src="https://user-images.githubusercontent.com/40908279/89699908-6c4aff00-d965-11ea-9e82-ddc397d4cf96.png">



