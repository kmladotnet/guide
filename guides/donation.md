# 기부물품 관리하기

## 기부물품 엑셀파일 업로드

* 원격서버에 ssh로 접속, /scripts/donation 에서 sample.xlsx 를 다운로드.-> scp 이용 (* 참고: https://codereader37.tistory.com/143)
* sample.xlsx 를 행정위에 전달후 정리된 최종본을 donation.xlsx로 동일한 dir에 업로드.
* insert.py 실행

## 기부물품 신청 날짜 변경

* kmlaonline Repository 에서 kmlaonline/src/content/util/donation-book.php 의 line 113, line 117의 날짜를 변경. 
* kmlaonline Repository 에서 kmlaonline/src/content/util/donation-cloth.php 의 line 100의 날짜를 변경.
