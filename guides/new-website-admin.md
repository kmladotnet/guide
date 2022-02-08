# 새로운 닷넷 멤버: 웹사이트 관리자 권한 주기

이 문서는 KMLA Online 웹사이트 유저에게 관리자 권한을 제공하는 방법을 설명합니다. 웹사이트 관리자는 각 게시판에 대해 사용자들의 접근을 관리할 수 있습니다. 노래방, 공강 등의 게시판 관리자 권한, 학생회 게시판의 글 작성 권한 등을 제어합니다. 

### Prerequisite
* 서버 sudo 권한
* 서버 MariaDB 비밀번호
* kmlaonline.net 유저 일련번호 (자신 프로필에 들어가면 URL에 숫자가 포함되어 있을 것임. 홈 > 정보 > URL에 있는 숫자)

## 설명

기본 유저는 DB에서 n_admin값이 0으로 시작합니다. 이 값이 1이 되면 관리자 권한을 사용할 수 있습니다. 

```bash
$ mysql kmlaonline -u kmlaonline -p
Enter password: <mariadb-password>

MariaDB [kmlaonline]> update kmlaonline_member_data set n_admin=1 where n_id=<user-id>;
Query OK, 1 row affected (0.002 sec)
Rows matched: 1  Changed: 1  Warnings: 0
```
