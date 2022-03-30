# Django Tutorial

Django 프레임워크를 이용한 Pybo (게시판) 만들기

* reference: 점프 투 장고 <https://wikidocs.net/book/4223>

## 주의

현재 Repository는 Public이므로 장고 Secret Key가 공개되어 있다. 따라서 본 코드를 그대로 사용하는 것을 금한다.

## Usage

### 가상환경 설정

```bash
$ conda create -n <venv name>
$ conda activate <venv name>
```

### 의존성 패키지 설치

* `bootstrap v5.x` 를 `static/` 밑에 다운로드
* `jquery` 를 `static/` 밑에 다운로드
* 아래 코드 실행

```bash
$ conda install django
$ conda install markdown
```

### 프로그램 초기화 및 시작

아래 코드 실행

```bash
$ cd <project home>

$ mkdir logs

$ python manage.py makemigrations
$ python manage.py migrate
```

### 시작

* mode: `local`, `prod`

```bash
$ python manage.py runserver --settings=config.settings.<mode>
```
