<center>
  
  <img src='https://github.com/Treeandsaw/KonicaRent/blob/master/konica.png'>
  
</center>


# KonicaRent
아미나 회원 테마 Konica Rent from Amina Theme

1. 기본파일 설치 <br>
그누보드 + 아미나

2. 아미나에서 받은 파일 설치  <br>
http://amina.co.kr/bbs/board.php?bo_table=skin_member&wr_id=9218

3. github에 필요한 파일 설치 <br>
https://github.com/Treeandsaw/KonicaRent
- img/home.png

4. 게시판 만들기 <br>
테이블명: rent <br>
스킨명: rent <br>
파일 업로드 개수: 8개로 수정 <br>

5. mapmarkers2.php 파일 수정

6. 첫화면 위젯 설정에서 가로에 3개씩 설정

7. 스타일 위젯에서 
- 페이지 설정: 1단 와이드

==================================
# Konica 2.0

중요파일은 아미나에서 다운로드 받아야 합니다.
http://amina.co.kr/bbs/board.php?bo_table=skin_member&wr_id=10093

그것을 받아도 부족한 파일이 있을경우 본 파일을 받아서 설치하세요.

@특징

1. 구글 지도에 하우스 마커 표시

2. 아래 여러 하우스들이 이쁘게 잘 나옴

3. 하우스 등록을 원하는 사람은 상단이 Listing을 클릭

4. 사람들이 코멘트도 달 수 있슴



@설치 법

일반 아미나 설치를 한 후 그 위에 앞축파일을 뒤집어 씌우면 됩니다. 

그 후 아래 파일만 수정해 주면 됨.

 깃헙에도 설명이 있음 : https://github.com/Treeandsaw/KonicaRent  



1. mapmaker2.php 

파일에 아래 내용 변경하기

  $username="root";

  $password="";

  $database="amina";



2. 구글 api 넣기

132줄 /map.php 

381줄 \skin\board\rent\list.skin.php:

279줄 \skin\board\rent\view\basic\view.skin.php:

607줄 \skin\board\rent\write\basic\write.skin.php:

<script async defer src="https://maps.googleapis.com/maps/api/js?key=<--put google api code here --->&callback=initMap"></script>  



3. 파일 구성내용

1. rent 게시판
2. google marker.php 파일
3. header, index, tail 부분의 디자인
4. latest 에서 집의 상세내용이 카드 형식으로 나오기 



4. 가격 비교 검색 수정 (안에 DB를 자기것으로 수정하세요.)

C:\xampp\htdocs\konica\compare.php:

   24  

   25      $servername = "localhost";

   26:     $username="koscccccccccica";

   27      $password="2Cbbbbbhe*^";

   28      $dbname = "kaaaaaaica"; 



5. 지도에 마커 표시되게 하기

C:\xampp\htdocs\konica\mapmarkers2.php:

<?php

  $doc = new DomDocument('1.0', 'UTF-8'); 

  $dom = new DomDocument('1.0', 'UTF-8');  



  $username="koaaaanica";

  $password="2bbbbbEhe*^";

  $database="kocccccca";



