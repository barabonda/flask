# flask
## Window VSCODE
flask 파일 만든 후
```from flask import Flask
app = Flask(__name__)

@app.route("/")
def home():
    return "Hello, Flask!"```
후에 `git clone <깃허브 주소>`

명령 프롬프트 켜서
python 설치
flask 설치
*환경변수가 설정되었기 때문에 다른위치에서도 되는 것
`python -m flask run --host=0.0.0.0 --port=5000`

## rinux
`git clone <깃허브 주소>`
sudo apt install python3-pip
`pip install flask`
`python -m flask run --host=0.0.0.0 --port=5000`

파이썬이 웹만을 위해 만들어진 시스템이 아니다보니
wsgi서버가 필요힘
*WSGI(Web Server Gateway Interface)
WSGI는 파이썬 웹 응용 프로그램을 위한 것이다. WSGI는 웹서버와 파이썬으로 작성된 웹 응용 프로그램 간의 표준 인터페이스를 말한다.
그 예로 **Gunicorn** 같은 것이 있

