# Pybo

## 실행 방법

### 1. 가상환경 실행

가상환경이 없다면 아래의 명령어로 만들면 된다.

```shell
python -m venv 가상환경이름
```

예를 들어 `python -m venv venv`로 실행하면 venv라는 이름의 가상환경이 만들어진다.
가상환경이 만들어졌다면 아래 명령어로 가상환경을 실행시켜준다. 폴더이름은 가상환경이름으로 만들어진다.

```shell
cd venv/Scripts
activate
```

이렇게 실행하면 프롬프트 앞에 (venv)가 뜬 것이 보이면 가상환경이 실행된 것이다.
진입한 가상환경에서 벗어날 때는 `deactivate` 명령어를 사용하면 된다.

### 2. 필요한 패키지 설치

```shell
pip install -r requirements.txt
```

```shell
pip install flask
pip install flask-migrate
pip install Flask-SQLAlchemy
pip install flask-wtf
```

### 3. 플라스크 애플리케이션 설정

디렉터리에서 `set FLASK_APP=pybo` 명령을 실행하여 환경 변수 FLASK_APP에 pybo라는 값을 설정해주어야 한다.

```shell
set FLASK_APP=pybo
set FLASK_DEBUG=true
```

### 4. 프로젝트 실행

```shell
flask run
```
