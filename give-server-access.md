# 새로운 관리자에게 서버 `Sudo` 권한 주기

## 🛑 정지
* Sudo 권한은 말 그대로 **모든 것을** 할 수 있는 권한
* 즉 키워드 하나 잘못 입력하는 순간 서버가 **터질 수 있음**
* 그러니 항상
    1) 중요한 정보의 백업을 해두고
    2) 테스트 서버에서 미리 안전을 확인할 것.
* 또한 다음 삼원칙을 명심할 것

```zsh
#1) Respect the privacy of others.
#2) Think before you type.
#3) With great power comes great responsibility.
```

## 새로운 서버 유저 추가

* 기존 Sudoer의 도움을 받아야함
* 다음 명령어를 이용해서 새로운 사용자를 추가하고 비밀번호를 설정해줌
* 처음에는 아이디와 동일하게 비밀번호를 설정하고, 새로운 유저는 바로 접속해 비밀번호를 변경해야 함
* wheel 그룹에 등록하는 것으로 sudo권한을 얻음

```zsh
➜ ~ sudo useradd -G wheel -m newuser -p newuser
```

## 비밀번호 설정 또는 변경

```zsh
➜ ~ sudo passwd newuser
New password: 
Retype new password: 
passwd: password updated successfully
```

## 또 하면 좋은 것
* GitHub KMLA Dotnet 팀에 추가해주기
* Linode에 새로운 멤버 가입시켜주기
    * 새로운 멤버가 회원가입을 직접 하는 것이 아님
    * [https://cloud.linode.com/account/users](https://cloud.linode.com/account/users)에서 기존 멤버가 직접 Add a User 눌러서 해줘야함
