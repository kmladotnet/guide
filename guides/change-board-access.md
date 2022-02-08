# 게시판 권한 수정하기

웹사이트 관리자는 게시판의 접근 권한 (글 읽기/쓰기/수정/삭제, 댓글 달기, 파일 업로드 여부 등) 수정할 수 있습니다. 이 글에서는 그 작업을 어떻게 수행하는지에 대해 설명합니다. 

> 관리자 메뉴는 홈 화면에 '관리자' 버튼을 클릭해 접근할 수 있습니다. 
> 관리자로 설정되어 있지 않다면 [새로운 닷넷 멤버: 웹사이트 관리자 권한 주기](/guides/new-website-admin.md) 매뉴얼을 참고하세요. 

## 메뉴 설명

* 사용자 관리: '분류 관리' 에서 개인 권한을 설정하기 위해 검색하는 창입니다. 
* 분류 관리: 각 게시판별로 개인 또는 기수별 권한을 조정할 수 있습니다. 
* 기타 권한 관리: 게시판이 아닌 큼라보드, 공강마스터 등의 권한을 부여/삭제할 수 있습니다. 

## 신입생 가입 시

* '분류 관리' 탭에서 새로 가입하는 기수를 선택한 뒤 다음과 같이 게시판 권한을 설정합니다. 

| 게시판 이름 | ID  | 권한 |
| ---------- | --- | ---- |
| 전체 공지사항 | 2 | 글 쓸 수 있음 |
| 전체 갤러리 | 3 | 글 쓸 수 있음 |
| 전체 자료실 | 4 | 글 쓸 수 있음 |
| 포럼 | 6 | 글 쓸 수 있음 + flag anonymous |
| 입법게시판 | 66 | 읽기 전용, 댓글 가능 |
| 사법게시판 | 67 | 읽기 전용, 댓글 가능 |
| 행정게시판 | 68 | 읽기 전용, 댓글 가능 |