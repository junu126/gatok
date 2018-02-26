---

layout: post

title: "깃헙 배우기_fourth"

---

<br>**♣본 포스팅은 PC에 최적화 되어있습니다.♣**

<br>

<h1>브랜치</h1>

<br>

<h3>브랜치란? 작업을 분기해서 할 수 있도록 도와주는 것.</h3>

<br>

&nbsp;&nbsp;&nbsp; -하나의 소스트리안에서 안정적인 작업과 안정적이지 않은 작업을 동시에 진행해야 하는 경우가 있을 수 있다.

<br>

&nbsp;&nbsp;&nbsp; -이런 상황에 Git의 Branch를 사용하면 아무런 불상사 없이 간편하게 병행할 수 있다.

<br>
<br>

<h1>브랜치 만들기</h1>

<br>

<h3>방법</h3>

<br>

<ul>
	<li>1. 새로운 브랜치를 추가할 버전을 클릭한다.</li>
	<li>2. 상단의 Branch를 누른다.</li>
	<li>3. New Branch라고 적혀있는 부분에 제목을 적는다.</li>
	<li>4. Create Branch를 누른다.</li>
	<li>5. 저장소에 브랜치가 생성된다.(좌측에 확인가능)</li>

<br>

<li>'브랜치'단계에서 들었던 예를 바탕으로 안정적인 작업을 진행한다면 master브랜치를 더블클릭해서 아이콘에 '체크'표시가 생기가 한후 진행하고,</li>

<br>

<li>안정적이지 않은 작업을 진행한다면 새로만든 브랜치드를 더블클릭을 하면된다.</li>

<br>

	<li>6. 작업을 마치고 꼭! commit을 한다.</li>
	<li>7. 그래프가 바뀜을 확인한다.</li>

</ul>

<br>
<br>

<h4>§안정적인 작업을 했던 것 들은 안정적이지 않은 작업에 나타나지 않는다.§</h4>
<h4>§각 작업마다 따로 저장이 된다고 생각하면 된다.§</h4>

&nbsp;&nbsp;&nbsp; -마치 두개의 디렉토리에서 각각 다른 파일들을 수정하는 것과 비슷한 느낌이 난다.

<br>

<h1>브랜치 합치기</h1>

<br>

<h3>브랜치를 사용하는 이유중 가장 중요한 이유중 하나가 브랜치를 합치기 위해서다.</h3>

<br>

<h3>예 : 만약 안정적이지 않은 작업이 성공적으로 진행되었다. 그래서 안정적인작업과 합치게 되었다. 어떻게 해야할까?</h3>

<h3>방법</h3>

<br>

<h4>**!이 방법은 안정적이지 않은 작업을 master로 옮기는 작업이다.!**</h4>

<br>

<ul>
	<li>1. 브랜치를 master브랜치로 체크 아웃한다.(체크아웃이란? 브랜치를 더블클릭해서 아이콘위에 '체크'표시가 나오도록 하는 행위)</li>
	<li>2. 원하지않는브랜치를 우클릭한다.</li>
	<li>3. Marge "이름" into current branch라고 적혀있는 부분을 누른다.</li>
	<li>4. 그래프의 변화를 확인한다.(두개의 그래프가 붙어있으면 성공이다.)</li>
	<li>5. 버전이 합쳐진 부분에 새로운 버전이 생긴다.</li>
	<li>6. Merge branch "이름"이라는 새로운 버전이 있어야 한다. (의미 : "이름"을 Merge로 병합한 버전이다.)</li>
	<li>7. Merge bracnh "이름"의 버전을 확인해 보면 앞에 '+'와 녹색으로 색칠되어 있는 단락이 "이름" 브랜치 이다.</li>

	<br>

	<li>두개의 브랜치는 공통의 '버전'으로부터 시작된다.</li>

	<br>

	<li>처음에 브랜치를 추가한 버전이 공통의 버전이 되는 것 이다.</li>
</ul>

<h1>브랜치간의 충돌의 해결</h1>

<br>

<h3>아주 많은 경우에 브랜치를 병합할때 충돌이 생긴다. 어떻게 해야할까?</h3>

<br>

<h3>충돌이란? 두 브랜치에서 서로 같은 곳을 수정했을 경우에 버전관리 시스템이 자동으로 병합해줄 수 없을때 직접 수정해야하는 경우.</h3>

<br>

<h2>방법</h2>

<br>

<ul>
	<li>1. 충돌이 일어난 소스코드를 확인한다.</li>
	<li>2. <<<<<<< head 와 =======로 이루어진 기호 사이에 있는 코드와 head가 좀전에 체크아웃한 브랜치이다. </li>
	<li>3. ========과 >>>>>>>"이름"으로 이루어진 기호 사이에 있는 코드와 "이름"은 "이름"이라는 브랜치 이다.</li>
	<br>
	<br>
	<li>4. 원하지 않는 부분의 브랜치는 삭제한다.</li>
	&nbsp;&nbsp;&nbsp; EX) <<<<<<< head
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<.li>brench<./li>
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=======
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<.li>brench2<./li>
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>>>>>>> "이름"
	<br>
	&nbsp;&nbsp;&nbsp; -만약 체크아웃하고있는 브랜치를 유지시키고 싶다면
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<.li>brench<.li>
	<br>
	&nbsp;&nbsp;&nbsp; - 저 부분만 남겨두면 된다.
	<br>
	<br>

	<li>5. 깃으로 돌아가서 Uncommitted changes로 가면 하단에 아이콘이 !로 변해 있다.</li>
	<li>6. Resove Conflicts에 있는 Mark Resolved를 클릭한다.</li>
</ul>

<br>

<h3>조금 어려운 내용이지만 이해할 수 있다!</h3>

<br>

<h1>브랜치 충돌의 예방</h1>

<h3>충돌을 억제할 수 있는 방법, 충돌이 작은범위에서 일어날 수 있도록 하는 방법을 알아보자.</h3>

<ul>
	<li>1. 새로운 브랜치를 만든다.</li>
	<li>2. master브랜치의 내용을 새로운 브랜치로 옮긴다.(Merge를 이용)</li>
	<li>3. 이후 새로운 브랜치에서 작업을 한다.</li>
	<li>4. 작업을 마치고 커밋한다.</li>
	<li>5. 다시 master를 체크아웃하고 작업을 계속 한다.</li>
	<li>6. 작업을 마치고 커밋한다.</li>
	<li>7. 다시 새로운 브랜치를 체크아웃해서 master의 작업내용을 병합한다.</li>
	<li>8. 이후 작업을 시작한다. 하지만 충돌이 일어난다.</li>
	<li>9. 충돌을 해결한다.(충돌을 막는 것이 아니라 완화시키는 것 이다.)</li>

	<br>

	<li>조금씩 계속 충돌을 해결해 나가면서 충돌을 완화시키는 방법이다.</li>
	<li>예방작업을 계속하면서 실질적으로 매번 충돌이 일어날 일은 없을 것이다.</li>

	<br>

	<li>10. 충돌을 해결하고 깃으로 돌아와서 Resolve conflicts - Mark Resolved를 클릭한다.</li>

	<br>

	<li>Resolve conflicts창에 여러 기능이 있는데 우리는 수동으로 편집했기에 Mark Resolved를 사용하는 것 이다.</li>

	<br>

	<li>Resolve Using 'Mine' 이란? 자신의 브랜치에 있었던 내용을 채택한다.</li>
	<li>Resolve Using 'Theirs' 이란? 자신의 것을 삭제하고 병합한 브랜치의 내용을 채택한다.</li>

	<br>
	<br>

	<li>11. 이후 master브랜치를 체크아웃 해서 병합한다.</li>

</ul>

<br>
<br>

**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">알게된 점.</a>**

<h4>브랜치에 대한 이론, 만드는 방법, 병합방법, 충돌 해결법, 완화법을 알 수 있었다.</h4>



**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">느낀점</a>**

<h4>지금까지 Git을 배우면서 제일 어려운 부분이었다. 하지만 나는 나아간다! Git을 마스터하기 위해!</h4>
