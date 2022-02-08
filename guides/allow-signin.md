# KMLA Online 웹사이트 가입하기

## 회원가입 활성화하기

* `src/content/user/login.php`의 [52번째 줄](https://github.com/kmladotnet/kmlaonline/blob/master/src/content/user/login.php#L52)을 주석 해제하면 회원가입 버튼이 활성화됨

## 회원가입 승인하기

* ssh, sftp 등의 클라이언트로 서버에 접속하기 ([서버 접속하기](/guides/connect-server.md))
* 신청서 위치(아래)로 접근해서 생성된 신청서 파일 (`txt` 확장자) 의 내용을 리뷰한 후 승인을 결정했다면 파일을 삭제
```
/srv/http/kmla/data/user_pending_list
```
* 신청서가 삭제된 회원은 가입이 승인됨
