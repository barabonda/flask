# flask
## Window VSCODE
flask 파일 만든 후
`from flask import Flask
app = Flask(__name__)`

@app.route("/")
def home():
    return "Hello, Flask!"

후에 `git clone <깃허브 주소>`

명령 프롬프트 켜서
python 설치
flask 설치
*환경변수가 설정되었기 때문에 다른위치에서도 되는 것
`python -m flask run --host=0.0.0.0 --port=5000`

## rinux
`git clone <깃허브 주소>`
파이썬이 깔려있다고 뜨지만 pip를 치면 안뜰거임 그래서
`sudo apt install python3-pip`를 하고
`pip install flask`
`python -m flask run --host=0.0.0.0 --port=5000`

파이썬이 웹만을 위해 만들어진 시스템이 아니다보니
wsgi서버가 필요힘
*WSGI(Web Server Gateway Interface)
WSGI는 파이썬 웹 응용 프로그램을 위한 것이다. WSGI는 웹서버와 파이썬으로 작성된 웹 응용 프로그램 간의 표준 인터페이스를 말한다.
그 예로 **Gunicorn** 같은 것이 있

github에
`if __name__ == '__main__':
    app.run('0.0.0.0', 5000, True)`

를 바꾸면 `python3 app.py` 만 눌러도 웹실행 가능
VSCODE, 리눅스 cmd
`git pull`
`python3 app.py`
`
방화벽 -> 고급설정 -> 새규칙 -> 포트 ->5000 다음
그러면 5000번 실행됌

##curl 명령어
`udo apt  install curl`
`curl 127.0.0.1:5000`

[curl 관련 레퍼런스]
https://inpa.tistory.com/entry/LINUX-%F0%9F%93%9A-CURL-%EB%AA%85%EB%A0%B9%EC%96%B4-%EC%82%AC%EC%9A%A9%EB%B2%95-%EB%8B%A4%EC%96%91%ED%95%9C-%EC%98%88%EC%A0%9C%EB%A1%9C-%EC%A0%95%EB%A6%AC



