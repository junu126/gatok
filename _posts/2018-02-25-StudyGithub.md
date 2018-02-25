---
layout: post
title: "깃헙 배우기_first"
---



<br>**♣본 포스팅은 PC에 최적화 되어있습니다.♣**





<br>
<h1>버전관리 란?</h1>




<h3>◎버전</h3>


<br>


&nbsp;&nbsp;&nbsp;-정의 : **어떠한 의미있는 변화들**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -기능의 개선, 버그수정, 커스터마이징 등

 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - 여러 클라이언트에서도 이용되고 있다.(Dropbox, Google Drive)

<br>

 <h1>Git과 SourceTree 설치</h1>



<h3>◎<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">Git과 SourceTree 다운 설명 링크.</a></h3>


<br>


<h1>Git 공부 - 예제 설명</h1>



<h4>

01 : `<.html>`
<br>
02 : &nbsp;&nbsp;`<.head>`
<br>
03 : &nbsp;&nbsp;&nbsp;&nbsp;<.meta charset="UTF-8" />
<br>
04 : &nbsp;&nbsp;&nbsp;&nbsp;<.title>GIT 수업<./title>
<br>
`05 : &nbsp;&nbsp;</head> `
<br>
`06 : &nbsp;&nbsp;<body>`
<br>
`08 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<header>`
<br>
`09 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<h1>Git</h1>`
<br>
`10 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</header>`
<br>
`11 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<ul>`
<br>
`12 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>sync.egoing</li>`
<br>
`13 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>introduce Git</li>`
<br>
`14 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>version</li>`
<br>
`15 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>Branch</li>`
<br>
`16 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>브랜치</li>`
<br>
`17 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>충돌</li>`
<br>
`18 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>충돌해결</li>`
<br>
`19 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>원격저장소</li>`
<br>
`20 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>push</li>`
<br>
`21 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>pull</li>`
<br>
`22 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>협업</li>`
<br>
`23 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>sync</li>`
<br>
`24 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>push.egoing</li>`
<br>
`25 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>pull.leezche</li>`
<br>
`26 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>conflict.egoing.leezche</li>`
<br>
`27 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>외부도구.master</li>`
<br>
`28 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>스테시</li>`
<br>
`29 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<li>ignore</li>`
<br>
`30 : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</ul>`
<br>
`31 : &nbsp;&nbsp;</body>`
<br>
`32 : </html>`

</h4>

<br>

- **깃을 공부하는데 예제가 어려우면 조금 힘들 수 잇기에 간단하고 쉬운 예제를 사용한다.**

<br>

- **각 코드앞의 '.'은 제외하고 읽는다.**



<h1>저장소 만들기 (init)</h1>



<h3>1. 소스트리를 실행</h3>



&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-**여러 버전관리시스템들을 사용하다보면 대부분 영어로 이루어져 있기에,**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**영어로 바꾸는 것을 추천한다.**



&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **-변경하는 방법은 <font color=green>도구-옵션-언어</font>에서 변경 가능하다.**



<h3>2. Repository(저장소) 만들기</h3>



&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-**좌측 상단의 '+' 버튼을 클릭**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-**상단의 메뉴에서 Add를 클릭**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-**위에서 아래로 차례대로 작업경로, 이름, 루트를 설정 **

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-**작업 경로에 자신의git Repositories의 주소를 적으면, 자동으로 이름이 입력됨.**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-**올릴 루트는 따로 변경하지 않아도 됨.**



**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">알게된 점.</a>**

<h4> 버전관리와 Git, SourceTree를 설치하는 방법을 알 수 있었고,GitHub에 올리기위한 저장소를 만드는 방법을 알았다.</h4>



**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">느낀점</a>**

<h4>대마고에 입학하게 되어서 처음으로 블로그를 만들고, 포스팅해보는데 생각보다 재밌고, 내가 공부한 내용을 기록할 수 있어서 행복한 것 같다. 앞으로 꾸준히 포스팅을 계속 할 수 있으면 좋겠다.</h4>

