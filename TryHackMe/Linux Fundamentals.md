# Part 1

- 명령어로 리눅스 머신 다뤄보기
- 파일 시스템을 다루는 데 필요한 리눅스 명령어
- 파일 검색과 쉘 연산자

## Running First Few Commands

- echo: 입력한 텍스트 출력(쌍따옴표는 사용 x)
- whoami: 현재 로그인하고 있는 사용자의 username

## Interacting with File System

- ls: 파일 열거
- cd: 디렉토리 이동
- cat: concatenate (파일 내용 확인)
- pwd: 작업 중인 디렉토리 출력
- find: 찾는 파일이 있는 디렉토리 출력 ex. find -name (파일 이름) 혹은 find -name *.(찾고자 하는 파일 확장자)
- wc: entry 개수를 세어 줌 ex. word count -l (파일명)
- grep: ex. grep "찾고자 하는 내용" (파일명)

## Shell Operators

- &: 백그라운드 실행 (다른 명령 실행 가능)
- &&: command1 && command2 둘 다 실행 (이때 command1이 제대로 실행되었을 때만 command2 실행)
- ">": output redirector ex. echo hey > welcome 이면 welcome이라는 파일에 hey가 저장됨
- ">>": ">" 연산자와 다르게 내용을 덮어쓰지 않고, 끝에 내용을 추가

---
