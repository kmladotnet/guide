# 새로운 관리자에게 서버 `Sudo` 권한 주기

## Sudo이란?

* 서버에서 Super-do 권한을 가진 사람을 이르는 말
* 일반적으로 닷넷 외부 인원이 Sudo 권한을 가진 Sudoer가 됨

```zsh
We trust you have received the usual lecture from the local System
Administrator. It usually boils down to these three things:

    #1) Respect the privacy of others.
    #2) Think before you type.
    #3) With great power comes great responsibility.
```

## 새로운 서버 유저 추가

* 기존 Sudoer의 도움을 받아야함
* 다음 명령어를 이용해서 새로운 사용자를 추가하고 비밀번호를 설정해줌

```zsh
➜ ~ sudo useradd newuser
```

## 비밀번호 설정 또는 변경

```zsh
➜ ~ sudo passwd newuser
New password: 
Retype new password: 
passwd: password updated successfully
```

## 새로 추가된 서버 유저에게 Sudo 권한 부여

* 새로 추가된 서버 유저의 이름을 Sudoers File에 추가해야함
* 기존의 Sudoer 중 한 명이 다음 명령을 통해 Sudoers에 접근

```zsh
➜ ~ sudo visudo
```

* `vi`를 통해서 Sudoers 파일이 열린 것 (기초적인 vi 사용법을 알아야 함)
* 아래로 내리다 보면 다음과 같은 구역을 발견할 수 있음

```zsh
##
## User privilege specification
##
```

* 새로 추가할 Sudoer의 아이디를 입력하고, 위에 있는 사람들과 동일하게 나머지 값들을 입력
* 저장 및 종료
* 사용자 변경은 `su - username`로 할 수 있음.