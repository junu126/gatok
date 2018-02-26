---

layout: post

title: "깃헙 배우기_final"

---

<br>**♣본 포스팅은 PC에 최적화 되어있습니다.♣**

<br>

<h1>협업하기</h1>

<br>

<h3>Git을 이용하면 여러 프로그램을 만들 떼 여러명과 협업해서 만들 수 있다. 어떻게 협업 하는지 알아보자.</h3>

<br>

<h3>상황 가정 : 만약 내가 혼자 프로그램을 진행해 왔다. 그런데 다른 사람이 내 프로그램에 Join해야하는 상황이 왔다. </h3>
<h3>함께 하게된 맴버는 원격저장소에 있는 내용을 그의 로컬저장소로 가져가야한다. 이때 사용하는 계념이 Clone(복제)이다.</h3>

<ul>
	<li>1. 로컬저장소를 하나더 만든다.(상단의 '+'아이콘을 클릭한 후 Clone을 클릭한다. 이후 첫번째 칸에 Github페이지로 가서 전에 만들어 두었던 원격저장소의 하단 우측을 보면 HTTPS clone URl이 있다. 소스를 복사해서 넣는다. 두번째 칸은 우측의 ...을 클릭해서 복제를 하고 넣을 폴더를 선택한다.)</li>

	<br>
	<br>

	<li>2. 만든 로컬저장소를 오른쪽 클릭한 후 Show in Explorer를 선택하면 Clone을 통해 로컬저장소로 원격저장소에 있는 내용을 옮겨 왔음을 알 수 있다.</li>
</ul>

<br>
<br>

<h1>Pull, Push</h1>

<br>

<h3>Pull이란? 원격 저장소의 내용을 로컬 저장소로 다운 받는 기능</h3>
<h3>작업하기 전에 원격저장소와 자신의 로컬 저장소를 같은 상태로 만들고 작업을 진행해야지 충돌이 일어날 가능성이 적다.</h3>

<br>

<h3>Pull 사용법</h3>

<br>

<ol>
	<li> Remote vranch to pull이라는 부분을 master로 설정하면 master브랜치를 현재 로컬브랜치인 master브랜치로 가져오겠다는 뜻이다.</li>
	<li> 확인을 누른다.</li>
</ol>

<br>

<h4>서로다른 두개의 로컬저장소를 각자 commit하고 push할때, 오류가 날 것이다.</h4>
<h4>예를 들어 ) 만약 1번 만을 push하면, 2번은 아직 push하지 않았으니 원격저장소와 다를 것이다. 이때 2번을 pull을 이용해서 원격저장소에서 1번의 로컬저장소 내용을 가져온다. 그러면 1번과 2번의 작업이 병합돼서 별도의 버전이 된다. 이제부턴 push를 할 수 있는 상태가 된다.</h4>

<br>
<br>

<h1>PULL , PUSH 정리</h1>

<br>

<h3>순서</h3>
<br>

**원격저장소가 잇고 협업하는 개발자가 있다면 어떠한 작업을 하기전에 반드시 Pull을 먼저하는게 좋은 습관이다.**

**이 방법 행동을 통해 원격저장소에  혹시 있을 버전을 자신의 로컬 저장소로 가져온 다음에 작업을 한다.**

<br>
<br>

<ol>
	<li>Pull</li>
	<li>작업</li>
	<li>Commit</li>
	<li>Pull</li>
	<li>Push</li>
</ol>

<br>
<br>

<h1>협업 - 충돌해결</h1>

<br>
<br>

<h3>지금까진 서로 다른부분을 수정할 때를 알아보았다.</h3>
<h3>하지만 이번에는 서로 같은 부분을 수정해서 충돌이 일어난 경우를 해결해보자.</h3>

<br>

<h3>협업에서도 기존의 충돌과 별 다를게 없다.</h3>

<p>
	&nbsp;&nbsp;&nbsp; EX) <<<<<<< head
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<.li>conflict.egoing<./li>
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=======
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<.li>conflict.leezche<./li>
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;>>>>>>> e2d711eeae265d49bc809ecb25e0f76a3da0d2c
	<br>
	&nbsp;&nbsp;&nbsp; - conflict.egoing이 자신의 로컬저장소의 버전, conflict.leezche가 다른 로컬저장소의 버전 이다.
	<br>
	&nbsp;&nbsp;&nbsp; - 만약 자신의 브랜치를 유지시키고 싶다면
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<.li>conflict.egoing<.li>
	<br>
	&nbsp;&nbsp;&nbsp; - 저 부분만 남겨두면 된다.
	<br>
	&nbsp;&nbsp;&nbsp; - 만약 둘다 남기고 싶은경우에는
	<br>
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<.li>conflict.egoing.leezche<.li>
	<br>
	&nbsp;&nbsp;&nbsp; - 이렇게 적고, 나머지를 제거하면 된다.
	<br>
	<br>
</p>

<br>

<h3>이후 충돌을 해결했으니 Uncommitted changes에 있는 충돌이 일어난 상태인 패일을 우클릭 해서 Rexolve Conflicts - Mark Resolved를 체크한다.</h3>
<h3>이후 다시 commit을 한다.</h3>

<br>
<br>

**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">알게된 점.</a>**

<h4>로컬 저장소가 한개가 아닐때 협업하는 방법과 협업으로 인해 생기는 충돌을 해결하는 방법을 알게 되었다!</h4>



**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">느낀점</a>**

<h4>아.. 아직 고등학교1학년이라 협업을 할 기회가 생길지는 잘 모르겠지만 앞으로 유용하게 쓰일 것 같고, Push와 Pull을 잘 이해할 수 있었던 것 같다.</h4>
