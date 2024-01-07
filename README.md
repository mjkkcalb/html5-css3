# HTML ****(Hyper Text Markup Language)****

- 페이지의 제목, 문단, 표, 이미지, 동영상 등 웹의 구조를 담당 (안에 들어있는 구조들만 작성)

- html 기본 문법
    1. <태그>내용</태그> = <h1>Hello world!</h1>
        
        • 이 전체를 요소(Element)라 부른다. 앞에 태그를 열린 태그라 하고, 뒤에 태그를 종료 태그라 한다.
        
    2. <태크 속성="값">내용</태그>
        
        • 속성(Atrribute) | 값(Value) -> 기능의 확장
        
    3. `<태그>`: 빈(Empty) 태그
    4. `<태그/>` : 태그를 시작하자마자 종료를 시킨다.
        
        

## **230824**

### 1. 제목 태그 < title >

- h1 : 문서의 메인 제목. 한 문서에 한 번만 사용하는 것을 권장. 주로 로고에 사용
- h2~h6 : 제목 태그로 한 문서 안에 여러 번 사용 가능.

### 2. 문단태그 p

- 블록 태그
- 블록 요소이나 문단 태그는 또 다른 블록 요소를 포함하지 않는다. 주로 인라인 요소에만 넣음.
- 하나 이상의 문장으로 구성되며 독립적인 단위 형성.  문단의 시작은 새로운 줄로 나타낸다
- • `<p>` 태그 안에는 인라인 태그(input, image, a...등) 빼고 들어갈 수 없다.
- 태그 구성: 요소 Element 속성 Attribute = “갑 Value”
    - Semantic Markup - 태그가 가진 의미에 집중하여 컨텐츠 자체에 의미를 부여하는 것. 웹 접근성 부부넹서도 중
    

### 3. 일반 강조 태그 em

- 인라인 요소
- 강조의 이미로 사용되며, 주로 기울여져서 표현.
- 디자인을 위해 em을 사용해서는 안된다.
- 비슷한 태그로는 [ i ] 가 있으며, [ i ]는 단순 구분을 위해 사용된다.

### 4. 강한 강조 태그 strong

- 인라인 요소
- 굵은 글씨로 강조하는 효과를 준다.

### 5. 콘텐츠 분할 div

- 가장 대표적인 블록 요소
- 구조를 나누기 위한 태그로 브라우저 상의 특징이 없음.
- 단순한 레이아웃 구성을 하기 위해 사용. (id, cslaa 속성과 함께 사용)
    - id : 유일하게 단독으로 사용.
    - class : 어디든 사용할 수 있다.
    

### 6. 콘텐츠 분할 span

- 가장 대표적인 인라인 요소
- 인라인으로 구조를 나누기 위한 태그로 브라우저 상의 특징이 없음.
- 주로 다른 텍스트와 구분하고 싶지만 적절한 태그가 없을 때 사용.(id, cslaa 속성과 함께 사용)

### 7. 줄바꿈 태그 br

- 빈 요소, 혹은 열린 태그로 종료 태그 없음.
- 인위적인 여백을 만들기 위해 사용하지 않으며 위치에 반드시 줄 바꿈이 필요한 경우에만 사용.
- 반응형 웹에서는 br 태그를 이용해 줄바꿈을 하기 보다는 span 태그 사용을 권장하는 편이다.

## **230825**

### 1. 사용자 정보 address

- 블록 요소
- `연락처, url, 주소, sns, 사업자명, 사업자번호` 등

```html
  <address>
   <p>경기도 수원시 팔달구 향교로 1번길 20<br>
   우)16455</p>
   <p>tel.031-895-5782</p>
  </address>
```

### 2. 순서 있는 목록 ol

- 블록 요소
- 순서가 필요한 리스트에 사용.
- <ol>과 <li> 사이에는 다른 태그가 올 수 없다.
- <li> 태그 안에는 다양한 태그들 작성 가능.
- <ol>과 <li> 는 함께 사용되며, 둘 중 하나만 사용할 수 없다.

### 3. 순서 없는 목록 ul

- 블록 요소
- 블릿 기로로 표기
- <ul>과 <li> 사이에는 다른 태그가 올 수 없다.
- <li> 태그 안에는 다양한 태그들 작성 가능.
- <ul>과 <li> 는 함께 사용되며, 둘 중 하나만 사용할 수 없다.

### 4. 정의형 목록 dl

- 블록 요소
- 정의형 목록 태그로 용어의 정의, 설명, 참고문헌, 메타데이터 등 다양하게 사용 가능
- 일부 os에서 dl의 정의가 다르기 때문에 접근성이 좋지 않음
- dl/dt/dd는 항상 같이 사용한다
- dl안에서 dd없이 dt단독사용도 가능하다.

```html
  <dl>
    <dt>dt: 항목의 제목, 용어..</dt>
    <dd>dd: 위의 제목이나 용어의 설명을 작성하는 부분</dd>
    <dd>dd는 하나이상 작성 가능</dd>

    <dt>html이란?</dt>
    <dd>하이퍼텍스트 마크업 랭귀지로, 웹문서의 구조를 담당한다.</dd>

    <dt>css란?</dt>
  </dl>
```

## **230828**

### 1.  Html5 Layout

- 기본 구성
    - header
    - main
    - footer

```html
<!-- html5 구조 -->
<div id="container" class="wrapper">
  div: 단순히 영역을 나누기 위해 주로 사용
  <header class="header">
    header: 페이지의 머리글. 제목, 로고, 메뉴, 검색 관련, 유틸리티, 로그인 등..
    <h1>h1: 페이지의 제목, 로고</h1>
    <nav>
      nav: 페이지의 내비게이션 영역(사이트내, 외부로의 이동). 메뉴, 목차, 색인...
      <ul>
        <li>메뉴1</li>
      </ul>
    </nav>
  </header>

  <main class="wrapper">
    main: 메인 컨텐츠 영역. 문서 내에서 *반드시* 한 번만 사용.<br>
    다른 header, footer, nav, article, section, aside의 하위로 작성할 수 없음.
    <article>
      <h3>article:</h3>독립된 컨텐츠. 제목 태그와 함께 작성. 게시판, 블로그, 뉴스 등의 영역
      <section>
        <h4>section:<h4>
        일반적인 문서 영역. 제목 태그와 함께 작성.
      </section>
    </article>
    <aside>aside: 간접 컨텐츠. 보조 컨텐츠</aside>
  </main>

  <footer>
    footer: 하단 바닥글. 회사정보, 저작권, 연락처...
  </footer>
</div>

```

### 2. 앵커 anchor

- `href` 속성을 이용하여 하이퍼 텍스트 설정
- `href` 속성을 통해 다른 페이지나 같은 페이지의 어느 위치, 파일, 이메일 주소와 그 외 다른 URL로 연결할 수 있는 하이퍼링크를 만든다.
- `<p>`태그를 이용하여 블럭설정하여 스타일을 주기도 한다.
- 주소를 임시로 작성할 경우에는 `""`는 빈칸으로 둘 수 없으므로, 임시 링크 기호 `#` 를 사용해 채워준다. (`#`는 `a태그`에서만 사용이 가능 / 임시 작성의 경우 클릭 시  해당 작성 페이지가 새로고침 된다)
- 새창으로 열기
    - 외부 사이트의 경우 `target`을 이용하여 꼭 새창으로 열기 해준다.
    - `a href`태그 뒤에 `target="_blank"` 추가
    
    ```html
    <p><a href="https://developer.mozilla.org/ko/docs/Learn/Getting_started_with_the_web/HTML_basics" target="_blank">MDN 사이트 바로가기</a></p>
    <p><a href="#">임시 링크</a></p>
    ```
    
- **URL이란?**
    
    : Uniform Resource Locator의 약자로 **웹 상에서 특정한 자원에 대한 주소**
    

### 3. 절대 경로 (외부 파일)

- 외부 사이트로의 이동시 사용
- 반드시 `http://` 혹은 `https://`로 시작하는 주소로 작성

## 230829

### 1. 상대 경로(내부 파일)

- 현재 웹페이지의 소속 폴더가 기준점으로 동인한 사이트 안에서의 내부 이동 시 사용.
- `./파일명.html` 혹은 `파일명.html`: 현재 웹페이지가 소속된 폴더
- `./디렉토리명/파일명.html` : 현재 웹페이지의 하위 폴더
- `../파일명.html` : 현재 웹페이지의 부모 폴더
- index.thml : 모든 웹 문서의 첫 페이지로 약속. 임의 변경 불가.
- 최상위 root 폴더 바로 아래 있는 index.html 문서만 첫페이지로 인식.

## 230830

### 1. 건너띄기 링크

* 특정 위치로 이동하는 태그

- anchor : 이동 태그
    - `"#"` 임시링크 기호
    - `href="#title"` 을 값으로 작성하면 동일한 이름을 가진 id 속성이 있는 태그 위치로 이동
        - ex) `<a href="#title1">초판 바로가기</a>`
    - 페이지 상단으로 이동하고자 할때
        - `<a href="#top">맨위로 #top</a>`
- id 속성 : 해당 문서 안에서 id들 중에 유일한 이름을 가진 식별자
    - 영어 소문자로 시작
    - _ , - , $ 을 제외한 특수기호 사용 불가
    - 공백(띄어쓰기) 불가
    - 숫자는 맨 첫음에 올 수 없음

### 2. 서브페이지 연결

- `<a href="./1_건너띄기링크.html">메인으로 돌아가기</a>` ->메인 페이지 상단 이동
- `<a href="./1_건너띄기링크.html#title5">메인의 제5판 바로가기</a>` ->문단으로 이동

## 230831

### 1. 이미지 img

- 인라인 요소
- 빈 요소, 빈 태그로 종료 태그 없음
- `src="이미지경로" alt="이미지 대체 텍스트"` 로 구성
- 컨텐츠로 분류되고 닫아주는 태그가 없음에도 범위를 가지며 가로 세로 값 조절이 가능하다.
- **img 성격**
    - 다른 인라인 요소와 만났을 때 하나의 글자, 단어처럼 인식.
- **figure과 figcaotion**
    - `<figure>` :이미지, 비디오 등의 컨텐츠를 구분할 때 사용.
    - 독립적인 컨텐츠. block요소.
    - `<figcaotion>` figure의 하위 요소로 부연 설명, 참조 태그. 반드시 figure 하위로만 존재.

### 2.﻿표 만들기 table

- table tr th td는 함께 작성해야 표가 만들어짐.
    - `<table>` : 테이블 작성시 시작을 알리는 태그
    - `<tr>` : 테이블의 행(줄)
    - `<th>` : 테이블의 셀(칸), 셀의 소제목
    - `<td>` : 테이블의 셀(칸), 일반적인 셀
- 테이블을 만들때, 각 줄마다 칸의 갯수(셀의 수)를 통일해야한다.
- 테이블을 만들 때 큰 구조를 먼저 만든 뒤 컨텐츠를 넣는게 좋다.

```html
 <table border="1">
    <tr><!-- 행(줄) -->
      <th>소제목</th><!-- 셀(칸) -->
      <td>셀</td>
      <td>칸</td>
    </tr>
    <tr>
      <td>1</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>테이블 셀의 크기는</td>
			<td>다른 셀의</td>
			<td>크기에 영향을 받는다</td>
    </tr>
  </table>
```

- 표 소제목 `th`
    - 각 셀들에 대한 대표성을 띄는 요소로 td와 동일하게 셀(칸)을 만들어 준다.
- 열 병합 `colspan`
    - colspan=column(열) + span 합성어
    - 뒤에 오는 셀(th, td)와 병합. 즉, 다른 열 colimn과 합침.
    - 병합한 뒤의 셀은 코드를 지워줘야 한다.
    - 지우지 않을 경우 셀의 숫자만 늘어나 뒤로 밀림 발생.
- 행 병합 `rowspan`
    - rowspan = row(행) + span 합성어
    - 아래에 있는 셀(th, td)와 병합. 즉, 다른 행 row와 합침
    - 가장 상단의 열에 합하고 싶은 값을 입력한다.
    - 병합한 뒤의 행에 열 코드를 지워줘야 한다.
    - 지우지 않을 경우 셀의 숫자만 늘어나 뒤로 밀림 발생.

### 3. 표 영역의 그룹화

- **caption**
    - table 전용 캡션
    - `<caption>`은 table 하위 요소로 반드시 table 요소와 함께 작성.(단독 사용 불가)
    - `<h2>``<p>``<div>`등과 같은 태그를 table 자식으로 쓸 수 없다.
    - 테이블 요소와 관련 없는 태그는 자식으로 쓸 수 없음.
- **`thead` 표의 머릿말**
- **`tbody` 표의 본문**
- **`tfoot` 표의 바닥글**
    - `thead`와 `tfoot`은 생략이 가능.
- 표의 영역을 그룹화 할 경우
    - 스타일을 주기 쉽다.
    - 웹 인쇄시 고정한 상태로 함께 출력.

## 230901

### 1. Form  기본

- form 관련 태그들 중 최상위 태그
- 폼 관련 태그들이 제대로 실행 되려면 form 태그를 반드시 작성 해야 함.
- `method="get"` : 간단한 데이터 전송 시 사용. 데이터가 주소 입력란에 표시되므로 보안 유지 안됨.
- `method="post"` : http 헤더에 숨겨져 서버로 전송. 일정 크기 이상의 데이터 전송 시 사용. 데이터가 주소 입력란에 표시되지 않아 보안 유지.
- `action="정보를 전송할 서버 주소"`

```html
  <form action="https://정보를 보낼 주소" method="get">
```

- `get`과 `post`의 차이는 주소창에 내용이 보여지는지, 보이지 않는지의 차이.

### 2. **input 태그**

> 참조 사이트 : https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input
> 
- 인라인 요소로 폼 안의 기본적인 필드 값을 만들 때 사용. 빈 요소
- input은 type 속성 값에 따라 역할이 달라짐.
    - `name="데이터 이름"`
    - `maxlength="value의 최대 수(문자수)"` →설정값 이상 작성 불가
    - `minlength="value의 최소 수(문자수)"` → 설정값 이하로 작성 불가
    - `placeholder="컨트롤 박스 안의 힌트"` → 컨트롤 박스 작성 전 기본 텍스트.
    - ``required="필수항목. 단, form 태그가 반드시 정의되어 있어야 함"`
    - `value="입력값, 출력값, 전송값"`
    - `autofocus="자동 포커스"`
    - `checked="체크박스 자동 선택"`
    - `selected="select 옵션 자동 선택"`
    - `disabled="비활성화"`
    - `autofocus` → 자동 커서
    - `required` →반드시 작성. 작성하지 않으면 넘어가지 않음.
    - `submit` → 전송
    - `reset` → 취소
    - `button` → 버튼
    - `value` → 내가 표시하고 싶은 값(이름) 작성한 내용으로 표현
    - `readonly` → 입력 필드가 읽기 전용
    
- 폼 그룹화 `fieldset`
- 같은 주제를 가지고 있는 폼 관련 요소를 그룹으로 묶어 구분지을 때 사용
    - `legend` : `fieldset` 요소의 제목
    - `fieldset` 요소 안에 작, 하나의 `fieldset` 안에 한번만 사용할 수 있다.

### 3.**이름표 label**

- 인라인 요소
- 폼과 관련된 요소에 이름표로 저장한다.
- `label` 요소를 정의함으로서 폼 요소와 연관 시킬 수 있다.
- 이름표 안에는 같이 묶음으로 보기 때문에 함께 동기화 된다.(이전에 사용자 입력 영역만 선택이 가능했다면, label로 묶여있는 내용 부분을 눌러도 선택이 가능하다.)
- 키보드를 통해 컨트롤이 가능하며 접근성이 향상된다.
- `<input id="one">`의 하나의 아이디 값과 `<label for="one">`의 for 값이 동일해야 연결 된다.

## 230904

### 1.video, audio 태그

- 웹 브라우저에서 플러그인 도움없이 재생
- 다양한 브라우저에서 재생될 수 있도록 하기 위해 source 태그를 사용
- 모던 브라우저에서는 video 태그만 작성해도 동작

```html
<video src="./video/flicker.mp4" autoplay muted loop controls poster="./video/flicker.jpg"></video>
```

- video 속성들:
    - `poster="대체 이미지. 영상을 불러오지 못하거나 불러오기 전에 보이는 이미지"`
    - `autoplay` → 자동재생(크롬의 경우 반드시 음소거가 되어 있어야 실행)
    - `muted` 음소거
    - `loop` 반복
    - `controls` 컨트롤 바
    - `preload` 재생 전 파일 미리 불러옴. `autoplay`와 함께 사용되는 경우 적용 안됨
- 오디오 태그는 요즘 많이 사용되지 않음.

```html
<audio src="./video/flicker.mp3" autoplay loop></audio>
```

### 2.favicon 연결

- favicon.ico
- 상단 태그 그림 =파비콘
- 가장 기본적인 파비콘 파일로 16X16 크기를 가짐.
- 일반적으로 파비콘 파일은 root 디렉토리 바로 아래 index.html 문서와 같은 위치에 둠
- favicon은 `head` 영역 사이에 작성한다.

### 3.meta 태그

```html
<!-- ** 문자 인코딩을 나타내는 '문자 집합 선언' -->
  <meta charset="UTF-8">
  <title>meta</title>
  <!-- HTTP 헤더가 제공하는 정보와 동일한 "프래그마 지시문"
	IE를 만나면 최신버전(Edge) 방식으로 렌더링 -->
  <meta http-equiv="X-UA-Compatible" content="IE=edge">

  <meta name="apple-mobile-web-app-title" content="meta">

  <!-- 문서 정보들
	전체 페이지에 적용되는 "문서 레벨 메타데이터" -->
	<meta name="title" content="meta 태그 공부">
	<meta name="description" content="설명: 메타 태그와 관련된 내용을 공부하는 웹문입니다.">
	<meta name="keywords" content="메타,웹문서,meta">

  <!-- 이전 방문 사이트 정보 추척
    "no-referrer-when-downgrade" https일 때만 전송
  -->
  <meta name="referrer" content="no-referrer-when-downgrade">
<!-- ** open graph -->
	<!-- 제목 -->
	<meta property="og:title" content="오픈 그래프 연습">
	<!-- 설명 -->
	<meta property="og:description" content="메신저나 sns, 블로그, 카페 등에 유용하게 사용됨">
	<!-- 이미지 -->
	<meta property="og:image" content="https://이미지주소">
	<!-- url -->
	<meta property="og:url" content="https://사이트주소">

  <!-- 트위터 -->
	<meta name="twitter:card" content="요약 내용">
	<meta name="twitter:title" content="제목">
	<meta name="twitter:description" content="설명">
	<meta name="twitter:image" content="https://이미지주소">
	<meta name="twitter:url" content="https://사이트주소">
```

- '~에 대해서'라는 의미를 가진 단어로 해당 html 문서가 어떤 내용을 담고 있으며, 문서의 키워드, 작성자 등으 알려주는 웹페이지의 요약
- `meta`: 문서 레벨 메타데이터 요소
- 표준 메타데이터 이름
- meta는 `head` 영역에 들어간다.

> 참고 site: https://developer.mozilla.org/ko/docs/Web/HTML/Element/meta
> 

### 4.오픈 그래프(Open Graph) 태그

```html
  <!-- og -->
  <meta property="og:title" content="오픈그래피 연습2">
  <meta property="og:description" content="오픈그래피 연습으로 깃허브 페이지를 통해 확인합니다">
  <meta property="og:image" content="https://kimmiri1234.github.io/og/images/code.png">
  <meta property="og:url" content="https://kimmiri1234.github.io/og/og.html">
```

- 링크 공유시 이미지와 간략한 내용으로 미리보기가 가능.
