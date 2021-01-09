# Coffee Shop Backend

## Getting Started

### Installing Dependencies

#### Python 3.8

python 3 최신버전을 install해주세요. [python docs](https://docs.python.org/3/using/unix.html#getting-and-installing-the-latest-version-of-python)

#### Virtual Enviornment

python dependency를 install 하기 전에 가급적
virtual environment를 활용하시길 바랍니다. [python docs](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/)

#### PIP Dependencies

virtual environment setup하고 running 하셨다면 
dependencies를 install 해주세요.
`/backend` 폴더에 가서 아래의 명령어를 입력해주시면 됩니다.

```bash
pip install -r requirements.txt
```

`requirements.txt` 안에 있는 패키지들이 install됩니다.

##### Key Dependencies

- [Flask](http://flask.pocoo.org/)  은 python의 backend microservices framework입니다. requests 와 responses를 처리하기 위해 이용됩니다.

- [SQLAlchemy](https://www.sqlalchemy.org/) 와 [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/) 은 Python SQL toolkit 이자 ORM 입니다. sqlite database를 핸들링 합니다. 

- [jose](https://python-jose.readthedocs.io/en/latest/) JWT를 encoding, decoding, verifying 하는데 사용됩니다.

## Running the server

virtual environment 가 돌아가는 상황하에 `./src` directory 가셔서 

flask app을 api.py로 지정하시고,

```bash
export FLASK_APP=api.py;
```

서버를 run 해주세요.

```bash
flask run --reload
```

`--reload` flag는 파일 변화를 탐지하고 서버를 리스타트 합니다.
