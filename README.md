# Find Music Start Time
# 사용법

##### import settings
##### from register import *
##### from fingerprint import *
##### from DB. setup_db import setup_db
##### from DB.fix_db import setup_fix_db
##### from recognise import *
##### from split import *

### 1. db를 생성한다.
setup_db()
setup_fix_db()

### 2. 고정음성의 대략적인 시간대를 입력한다.
store_time(라디오 프로그램 이름, 고정음성 이름, 시작시간(s), 종료시간(s), 순서)

### 3. 고정음성을 등록한다.
register_song(music_path, program_name, name)


### 4. 주어진 메인 음성을 split한다.
split(song_path, program_name, save_path)
