---

layout: post

title: "깃헙 배우기_fifth"

---

<br>**♣본 포스팅은 PC에 최적화 되어있습니다.♣**

<br>

<h1>원격 저장소</h1>

<br>

<h3>원격 저장소란? 지금까지 저장했던 저장소는 로컬저장소 였다. 인터넷 또는 네트워크에 연결된 어떤 컴퓨터에 또다른 저장소가 있고, 로컬저장소를 원격저장소에 연결해서 소중한 소스또는 버전들을 원격저장소에 백업을 할 수있는 기능이 있다.</h3>

<br>

<h3>원격 저장소를 사용하는 가장 큰 이유는 '백업'이라고 할 수 있다.</h3>

<br>
<br>

<h1>원격저장소 종류</h1>

<br>

<h3>원격저장소를 만드는 방법은 다양하다.</h3>
<h3>먼저 직접 서버를 구축하고 직접 저장소를 만든다음에 로컬저장소와 연결하는 방법과,</h3>
<h3>Git의 서비스를 이용하는 방법이다.</h3>

<br>

<ul>
	<li>1. Github을 이용한다. 오픈소스에 한해서 무료, private일 경우 유료. https://github.com/</li>
	<li>2. GitLab를 이용한다.(https://about.gitlab.com/) 저장소 제한없음. Unlimited Private Collaborators. 약간 불안정한 기억?!,내 서버에서도 설치할 수 있는 기능 제공. </li>
	<li>3. Yobi를 이용한다. Nhn 제작. 위와 비슷한 기능 (http://yobi.io/)</li>
</ul>

<br>

<h1>원격저장소 만들기</h1>

<br>

<h3>Github에서 오픈소스를 진행하는 방법</h3>

<br>

<ul>
	<li>1. Sign in을 눌러 로그인을 한다.(없으면 만든다.)</li>
	<li>2. New repository를 눌러서 새로운 저장소를 만든다.</li>
	<li>3. Repository name에 이름을 적고 Public으로 설정한다.</li>
	<li>4. 원격저장소가 깃헙에 개설되었다.</li>

	<br>

	<h3>원격저장소와 로컬저장소를 연동시킨다.</h3>

	<br>

	<li>1. 상단의 여러옵션중 Repository - Add Remote...를 누른다.</li>
	<li>2. add를 클릭한다.</li>
	<li>3. 깃헙으로 이동을 한 후 중상단에있는 Quick setup — if you’ve done this kind of thing before 에서 HTTPS로 맞춘 후 URL을 복사한다.</li>
	<li>4. 소스트리로 돌아와서 URL / Path에다가 붙여넣기를 한다.</li>
	<li>5. 우측의 Default remote를 체크한다.</li>
	<li>6. 항목에 추가한다.</li>

	<br>

	<h3>원격 저장소와 로컬 저장소가 연결된 상태이다.</h3>
	<h3>하지만 아직 둘은 동기화 되어 있지않다. 동기화하는 방법을 알아보자.</h3>

	<br>

	<li>1. 상단의 Push를 클릭</li>
	<li>2. 여러개의 브랜치 중에서 업로드 하려는 브랜치를 선택한다.</li>
	<li>3. OK를 누르면 '인증이 필요하다' 라는 창이 뜬다.</li>
	<li>4. Github의 아이디와 페스워드를 입력한다.</li>
	<li>5. Pushing 아래에 녹색바가 생기면 성공, 붉은색 바가 생기면 실패이다.</li>
	<li>6. Github으로 돌아와서 새로고침을 하고 동기화를 확인한다.</li>
</ul>

<br>

<h3>깃헙 페이지에서 중앙의 commits을 누르면 지금까지 했던 commit들을 확인할 수 있다.</h3>
<h3>우측의 Graphs를 클릭하면 프로젝트의 여러가지 변경 점 , 변경 사항들을 시각화해서 볼 수 있다.</h3>

<br>
<br>

<h1>원격저장소로 업로드</h1>

<br>

<h3>로컬 저장소에서 작업한 내용을 원격저장소로 업로드 하기</h3>

<br>

<ul>
	<li>1. 만약 로컬저장소에서 어떤 버전을 만들었고, Commit을 했다면 상단의 Push에 '1'이 뜬다.</li>
	<li>2. master가 있는 버전은 로컬저장소, Origin master가 있는 버전은 원격저장소에 저장되어 있다고 생각 할 수 있다.</li>
	<li>3. master가 있는 버전들을 원격저장소로 보내기위해 Push를 통해 보낸다.</li>
	<li>4. Origin master와 master가 같은 버전을 가르키고 있다. 라는 것을 확인한다.</li>
</ul>

<br>
<br>

**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">알게된 점.</a>**

<h4>원격저장소와 로컬저장소의 이론을 알게 되었고, 원격저장소에 업로드하는 방법을 알 수 있었다.</h4>



**<a hraf="https://www.youtube.com/watch?time_continue=1&v=N_rpDCZxRCY" target="blank">느낀점</a>**

<h4>사실 원격저장소에 업로드 하는 방법은 미리 알고 있었던 방법이다. 그렇기에 지금 이렇게 블로그 포스팅을 할 수 있기도 하다. 하지만 여러 이론들이나, Commit보는 방법등은 처음안 내용이라 유익했던 것 같다.</h4>
