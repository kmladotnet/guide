# KMLA Online 가입 승인하기

* `src/content/user/login.php`의 [52번째 줄](https://github.com/kmladotnet/kmlaonline/blob/master/src/content/user/login.php#L52)을 주석 해제하면 회원가입 버튼이 활성화됨
* FileZilla 등의 `sftp` 클라이언트를 다운로드
* 다음의 정보를 입력한 후 `Quickconnect`를 누름

|Host                 |Username     |Password     |Port|
|---------------------|-------------|-------------|----|
|sftp://kmlaonline.net|Your username|Your password|220 |

* 다음 위치로 접근해서 생성된 신청서 파일 (`txt` 확장자) 의 내용을 리뷰한 후 승인을 결정했다면 파일을 삭제

```
/srv/http/kmla/data/user_pending_list
```

* 신청서가 삭제된 회원은 가입이 승인됨
