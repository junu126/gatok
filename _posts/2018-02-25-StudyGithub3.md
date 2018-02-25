---

layout: post

title: "깃헙 배우기_third"

---

<br>**♣본 포스팅은 PC에 최적화 되어있습니다.♣**

<br>

<h1>되돌리기</h1>

<br>

<h3>보는 것 뿐만 아니라 과거의 특정한 상태의 코드로 돌아갈 수 도 있어야한다.</h3>

<br>

<h3>이번엔 버전관리시스템을 이용해서 과거의 코드로 돌아 가는 방법을 알아본다.</h3>

<br>

<h1>WorkingCopy Index Repository</h1>

<br>

<ul>
	<li>최초로 Commit을 하기 전 까지는 추가된 파일은 버전관리를 신경쓰지 않는 파일이다.</li>

<br>
<br>

	&nbsp;&nbsp;&nbsp; - 만약 저번에 만든 저장소에 README.md 파일을 추가하고 그 내용을 "나는 빡빡이다"라고 적는다면 소스트리에 README.md 파일이 추가될 것이다. 하지만 README.md파일의 앞에는 ? 가 붙은 원이 있을 것이다.

<br>
<br>

	&nbsp;&nbsp;&nbsp; - 이것은 최초로 Commit을 하지 않아서 이다. README.md파일을 커밋 한다면 다시 동그라미 않에 점이 3개있는 모양(modefied)으로 바뀔 것 이다.

<br>
<br>

	<li>저장소에 있는 index.html의 변화만을 하나의 버전으로 만들려면 어떻게 해야할까?</li>

<br>
<br>

	&nbsp;&nbsp;&nbsp; - index.html파일만 체크해서 버전으로 저장하면 된다. 체크하는 행위를 "add"라고한다.

<br>

	&nbsp;&nbsp;&nbsp; - 방금의 예제로 인해 하단의 공간과 상단의 공간의 차이점을 알 수 있다.

<br>

	&nbsp;&nbsp;&nbsp; - 하단은 수정 된 파일들의 목록이 표시되는 공간이다. Git에서는 "working copy"라고 부른다.

<br>

	&nbsp;&nbsp;&nbsp; - 상단은 Commit 버튼을 클릭 했을때 하나의 버전에 포함될 내용들이 표시되는 공간이다. Git에서는 "index" , 'staging area'라고 부른다.
</ul>

<br>
<br>

<h1>되돌리기 기능</h1>

<br>

<h3>만약 index.html파일을 수정했다.</h3>
<h3>하지만 다시 파일을 되돌리고 싶다.</h3>
<h3>어떻게 해야할까?</h3>

<br>
<br>

<ul>
	<li>소스트리의 index.html파일을 클릭하면 우측에 작성한 코드들이 뜬다.</li>
	<li>이때 붉은색으로 표기되고 -가 붙어있는 라인들이 수정한 내용이 원래 파일에서 삭재되었다는 뜻이다.</li>

<br>

	<li>이럴때 사용하는 것이 "Discard"버튼이다.</li>
	<li>Discard버튼을 클릭하면 현재 수정한 파일의 리스트가 나온다.</li>
	<li>Discard Changes를 누르면 '되돌리기'가 실행된다.</li>

<br>
<br>

	<li>꼭 Commit하기전에 작성했던 코드들을 비교해보는 습관을 들이자.</li>
</ul>
