
# HTML ****(Hyper Text Markup Language)****

- 페이지의 제목, 문단, 표, 이미지, 동영상 등 웹의 구조를 담당 (안에 들어있는 구조들만 작성)

- html 기본 문법
    1. <태그>내용</태그> 
        
        • 이 전체를 요소(Element)라 부른다. 앞에 태그를 열린 태그라 하고, 뒤에 태그를 종료 태그라 한다.
        
    2. <태크 속성="값">내용</태그>
        
        • 속성(Atrribute) | 값(Value) -> 기능의 확장
        
    3. `<태그>`: 빈(Empty) 태그
    4. `<태그/>` : 태그를 시작하자마자 종료를 시킨다.
        
        
- 웹페이지 분석
    
    ```html
    ex1)
    <div class="container>
    	<header></header>
    	<nav></nav>
    	<div class="contents"></div>
    	<footer></footer>
    </div>
    ```
    
    ```html
    ex2)
    <div class="container>
    	<header></header>
      <nav></nav>
      <div class="contents"></div>
      <footer></footer>
    </div>
    ```
    
    - main은 html 안에서 1번만 쓸 수 있다. 추가로 main의 부모 요소로 가능한 태그는 div or body 가 있다.
    - article → 독립적인 요소 / 제목 태그 필수( section과 차이 찾아보기)
    - section → 간편히 분할 해주는 요소 / 제목 태그 필수
    - 
- font
    
    > [https://caniuse.com/](https://caniuse.com/)
    > 
    - 위 사이트를 통해 신규 코드를 웹 브라우저에서 사용할 수 있는지 확인 가능하다.
    
    > *https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight#common_weight_name_mapping*
    > 
    - 위 사이트를 통해 폰트 weight 사이즈 확인 가능.
- swiper 사용
    - swiper 사이트 →[swiperjs.com](https://swiperjs.com/demos#autoplay)
    - demos 페이지에서 원하는 스타일 코드 열기
    - html과 css에 원하는 스타일 css와 js 외부 링크 파일 연결하기
    - 열어놓은 스타일 코드를 참고해 넣기
    - 10/17일 수업 자료 참고하기

- button → 전송을 시켜 결과를 받아야 할 때 사용
- 구글 폰트 아이콘 사용 시 ****Static icon font**** 은 복사해 title 아래로 넣고 ****Inserting the ico**** 은 넣고싶은 위치에 복사해 넣는다
- 드래그 컨트롤 +k+ f = 정렬

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
- ol과 li 사이에는 다른 태그가 올 수 없다.
- li 태그 안에는 다양한 태그들 작성 가능.
  ol과 li 는 함께 사용되며, 둘 중 하나만 사용할 수 없다.

### 3. 순서 없는 목록 ul

- 블록 요소
- 블릿 기로로 표기
- ul과 li 사이에는 다른 태그가 올 수 없다.
- li 태그 안에는 다양한 태그들 작성 가능.
- ul과 li 는 함께 사용되며, 둘 중 하나만 사용할 수 없다.

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

- favicon 적용 방법
    
    > [https://realfavicongenerator.net/](https://realfavicongenerator.net/)
    > 
    - 위 사이트에서 이미지를 만들고 난 뒤 저장해 사용할 사이즈에 맞는 이미지들은 html 파일 내부에 있는 images 파일에 저장한다. 추가로 site.webmanifest 문서는 html과 동일한 파일에 넣는다.
    
    ```html
    <!-- <link rel="shortcut icon" href=""> -->
      <link rel="apple-touch-icon" sizes="180x180" href="./images/apple-touch-icon.png">
      <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
      <link rel="icon" type="image/png" sizes="16x16" href="./images/favicon-16x16.png">
      <link rel="manifest" href="/site.webmanifest">
      <meta name="theme-color" content="#ffffff">
    ```
    
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
---
# **CSS (Cascading Style Sheets)**

### 1. CSS 기본

- 첫 시작 :  @charset “utf-8”;
- 기본 구조 : 선택자(selector) { 속성 (property) : 값 (value); }
- 주석 /**/
- shift+alt+방향키 → 복사

> [CSS Tools: Reset CSS (meyerweb.com)](https://meyerweb.com/eric/tools/css/reset/) - 기본 css 사이트
> 

### 2. 선언 방식

- 외부 선언
    - : css style 내용을 css 파일로 따로 저장하여 페이지를 연결시키는 방법
    - 여러개의 파일을 연결시킬 수 있기  때문에 공동/자주 사용되는 부분을 따로 저장하여 사용하는게 용이
    - <head>안에 <link>로 작성 /  <link rel=”stylesheet” href=”common.css”>
- 내부 선언
    - <head> 안에 <style>로 선언. / <style></style>
    - • `style` 태그 안은 CSS 영역.
- 인라인 선언
    - 각 html 태그에 직접 style 속성 값으로 지정.
    - 제어가 어렵다는 단점이 있어 잘 사용하지 않음.
    - style="특성:값” / <strong style=“font-size:14px; color:blue;”>텍스</strong>

### 3. CSS 상속

- 지정된 요소뿐만 아니라 자식, 자손 요소에게까지 적용되는 성격.
    - 폰트 관련 속성은 상속된다.
    - 배경색이나 배경 이미지 등의 속성은 상속되지 않는다.
    - 박스 모델 관련 속성은 상속되지 않는다.

### 4. 우선 순위

- **다른 종류의 선언문이며 같은 선택자인 경우**
    - in-line > 내부 선언 > 외부 선언의 순서로 우선 순위를 가짐.
- **같은 이름 혹은 같은 종류의 선택자 혹은 같은 종류의 속성인 경우**
    - 위에서 아래로 순차적으로 적용이 되고, 마지막에 선언된 스타일이 우선 순위 가짐.
- **같은 선택자가 아닌 다른 종류 선택자인 경우**
    - !important > inline > id(5) > class(3) > type(1) 의 순서로 우선 순위를 가짐.
    - 복합 선택자일때 각 점수를 합해 큰 값이 표현된다.

### 5. 선택자

- 일반 형제 선택자
    - 선택자 ~ 선택자
    - 기준 요소 뒤에 오는 모든 형제 관계 선택자
- 인접 형제 선택자
    - 선택자 + 선택자
    - 기준 요소 바로 뒤에 오는 형제 관계 선택자 단 하나만
- 자 선택자
    - 선택자 > 선택자

## 230906

### 1. Font **와 Text**

- **서체 사용시 주의사항**
    - 정확한 서체명 작성( 띄어쓰기 인용부호 대소문자 등)
    - 상대방의 컴퓨터에 서체가 없는 경우를 대비해 3-4개 서체를 추가 작성(fallback fonts)
    - 바탕체 종류로 끝나는 경우 제일 마지막은 serif로 작성
    - 돋움(고딕)체로 끝나는 경우 제일 마지막은 sans-serif로 작성
    - 1. 웹의 기본단위값 : px
- **폰트 사용 시 고려 사항**
    - 폰트 라이선스는 해결 여
    - 힌팅 폰트로 제작 여부
- **font와 text 특성**
    - `font-family`: 서체 종류
        - 대체 글꼴 작성 필요.
        - 돋움, sans-serif  & 바탕, serif 로 마지막에 글꼴을 정의.
    - `font-size`: 서체 크기
    - `font-weight`: 서체 굵기
        - normal, bold, 100~900값으로 설정.
    - `font-style`: 서체 스타일
        - normal, oblique, italic(기울여쓰기)
    - `text-transform`: 대소문자
        - 영문에서 대.소문자 관리. 한글은 대소문자가 없으니까 적용안됨.
        - `lowercase`: 전부 소문자
        - `uppercase`: 전부 대문자
        - `capitalize`: 모든 단어의 첫글자 대문자
    - `text-decoration`: 밑줄 및 취소선
        - `overline`: 글자 상단에 밑줄
        - `line-through`: 글자 중간에 밑줄. 취소선
        - `underline`: 글자 하단에 밑줄
        - `dashed`: 밑줄에 점선
        - `none`: 효과 전체 삭제
    - `text-indent`: 들여쓰기/ 내쓰기. 내쓰기를 주로 많이 
    쓴다.
        - `text-indent: 100px;` 첫 문장만 들여쓰기
        - `text-indent: -120px;` 첫 문장 내쓰기. 웹 문서 바깥쪽으로 이동.
    - `text-align`: 문자 정렬
        - `left`: 왼쪽
        - `right`: 오른쪽
        - `center`: 중앙
        - `justify`: 양 끝 기준 정렬. 이미지 정렬에 적합
    - `text-shadow`: 서체 그림자
        - `text-shadow` 작성시 반드시 띄어쓰기를 해야하며 ,를 사용하지 않는다.
        - (x축, y축, 번짐, 색상) 값 순으로 작성.
    - `line-height`: 줄과 줄 사이 간격. (행간)
        - `line-height: px;` ->웹의 기본 단위 값 = px, 폰트사이즈가 변경될때 계속 고정되어 있는 값으로 나타나기때문에 행간에서는 px을 거의 사용하지 않음.
        - `line-height: em;`
        - `line-height: 1.7;`
    - `letter-spacing`: 글자와 글자 사이 간격. 자간.
    - `word-spacing`: 단어와 단어 사이 간격. 어간.

## 230907

### 1. 마우스 이벤트: `<a>` 태그 스타일 주기

- `:`, `::`
    - 가상 선택자로 다양한 종류가 있으며 주로 실제하는 요소와 함께 작성.
    - 예) 의사 클래스, 의사 요소, 수열 선택자...
    - :link, :visited, :hover, :focus, :checked ...
    - 최근 만들어진 스타일은 `::` 두개를 사용하는 경우가 많다.

```html
    a:link{ 링크 상태일 때 }
    a:visited{ 방문했을 때 }
    a:hover{ 마우스를 위에 올렸을 때 }
    a:active{ 클릭했을 때 }
    [required]:focus{ 포커스(커서가 보이는 상태)되었을 때 }
```

### 2. `<form>` 요소 스타일 주기

- form 관련 요소들은 기본 스타일이 존재하기 때문에 직접 적용

### 3. 인라인 세로 정렬 `vertical-align`

- 서체 및 인라인 요소 세로 정렬 기준
- 글씨와 이미지 및 input의 정렬 상태가 맞지 않는다면, 이미지 요소 및 input에 `vertical-align`적용
    - `top` :현재 요소와 자손들 모두 top 기준. 단, 텍스트는 행간이 존재하기 때문에 상단 여백이 남음.
    - `baseline` :기본값
    - `bottom` :현재 요소와 자손들 모두 bottom 기준
    - `middle` :부모 기준(baseline 기준으로 글자 높이의 반)

### 4. 가로 세로 영역 제어 `width`, `height`

1. 블록 요소(p, div, h1, header, main, article, form, ul...)
    - 가로 값의 경우 부모 요소의 가로 값을 받음
    - 일반적인 흐름에서는 블록 요소 옆에 다른 요소가 올 수 없음
    - 자식으로 블록, 인라인 요소 등 대부분이 올 수 있음
    - 세로 값의 경우 자식 요소의 높이 값을 그대로 가져 옴
- `width`, `height`로 제어 가능
1. 인라인요소(span, img, a, em, input, strong...)
    - 가로 값의 경우 자식(컨텐츠)의 값을 가져 옴
    - 인라인 요소 옆에 다른 인라인 요소가 올 수 있음
    - 자식으로 인라인 요소만 올 수 있음
    - 세로 값의 경우 자식 요소의 높이 값을 그대로 가져옴
    - `width`, `height`로 제어 불가능

---

1. 고정 너비

- px을 이용해 너비를 설정. 고정값.
- `width: 500px; height: 300px;`
1. 가변 너비 _ % 를 이용해 페이지 내 백분율 단위로 표현. 페이지 사이즈에 따라 변한다. 요즘은 사용하는 디바이스가 다양하기 때문에 더 많이 씀.
    - `width: 70%;`
    - `height: 50%;`
        - % :상대단위.
            - width-> 부모를 기준으로 100분의 70.
            - height-> 부모를 기준으로 100분의 50.
        - 세로 %는 부모의 높이 값이 정의되어 있는 경우에만 적용 됨. 기본값일 때는 적용X .

## 230908

- p, div, h1, #id, .class
    
    : 다중 선택자: 여러 선택자에 동일한 특성을 부여하고자 할 때 사용. 쉼표로 구분. 띄어쓰기 상관없음 
    

## 1. 테두리 border

- 방향 지정 없이 입력 가능.
- 방향을 따로 입력하면 입력한 영역에만 스타일이 나타난다.
    - `border-width` 테두리 굵기
        - `border-(top, right, bottom, left) -width: px;`
    - `border-style` 테두리 스타일
        - `solid` : 기본선
        - `dotted` : 도트선. 점선
        - `double` : 이중선. 두줄. 3px 이상에서 사용
        - `dashed` : 대쉬선. 점선
        - `groove` : 입체선.
    - `border-color` 테두리 색상.
- 축약형: 값의 순서에 상관없이 띄어쓰기 구분.
    - `border: 8px ridge #ffbb5c;`
- override: 간결하게 작성

```
.box {
  border: 6px solid #000;
  border-bottom-style: double;
}
```

- `border`와 달리, `outline`은 요소의 바깥 부분에 그려지고, 요소가 가지는 실제 크기에 영향을 주지 않음.
- 다른 요소의 영역을 침범할 우려가 있어서 잘 사용하지 않는다.

### 2. 둥근 모서리 border-radius

- top-left, top-right, bottom-right, bottom-left순으로 각모서리마다 다른값을 줄 수 있다.
    - `border-radius: 50px 20px 50px 20px;`
- 서로 마주보고 있는 값을 한자리로 인식해서 적용.
    - `border-radius: 50px 20px;`
- 영역 밖으로 내용이 넘칠 때는 `overflow`를 이용해 숨길 수 있다.
    - `overflow: hidden;`

### 3. 안쪽 여백 padding

- 콘텐츠 영역과 테두리 사이의 여백
- 시계방향의 값을 가진다.
    - `padding: 0px 0px 0px 0px;`
- top+bottom=40px, right+left=20px 서로 마주보고 있는 값을 같이 작성 가능.
    - `padding: 40px 20px;`
- right+left=20px 서로 마주보고 있는 값. 같으면 생략해도 적용된다.
    - `padding: 30px 20px 40px;`
- 모두 같을때 하나의 값으로 작성 가능.(용량면에서는 기본 작성이 더 효율적)
    - `padding: 50px;`

### 4. 바깥 여백 margin

- 기준 요소의 바깥 여백을 말한다.
- 시계방향의 값을 가진다.
    - `margin: 0px 0px 0px 0px;`
- 서로 마주보고 있는 값을 같이 작성 가능.
    - `margin: 0px 0px;`
- right+left = 같은 값.
    - `margin: top px right+left px bottom px;`
- 모두 같을때 하나의 값으로 작성 가능.
    - `margin: 0px;`
- body에도 기본 margin값이 설정되어 있다.
- 단, 다른 박스는 padding에만 이미지나 배경색이 적용되는데, body의 경우 예외적으로 padding+margin까지 이미지나 배경색이 적용된다.
- **마진 상쇄 현상**
    
    :일반적인 흐름일 때 (단, float, flex, overflow, position등의 값이 적용된 경우는 발생하지 않음.)
    
    1. 형제 관계 요소에서 top과 bottom이 만낫을때 둘 중 큰 값이 적용됨. 
    
    2. 부모 자식 관계 요소에서 margin-top의 값이 같이 들어간 경우 둘 중 큰 값이 적용
    

### 5. 블럭 요소 중앙 정렬

1. 요소의 가로 값이 필요.
2. left+right값은 항상 auto로 설정.

```
.box {
  margin: 0 auto 0 auto; /* top right bottom left */
  margin: 20px auto; /* top+bottom=20, right+left=auto */
  margin: auto; /* 일반적인 상황의 auto=>가로 중앙 정렬만, 세로 중앙 정렬은 하지 않는다. */
  margin: auto 0; /* 세로는 오토가 먹지 않아서 값이 변하지 않음 */
  margin: 20px auto 0; /* top right+left bottom */
}
```

- "한 줄인 경우" 세로(위아래) 중앙 정렬 방법
    - `height`와 `line-height`의 값을 동일하게 적용
    - 영역에서 글이 두 줄 이상, 폰트 사이즈의 크기가 큰 경우는 잘 안됨.

```
.wrapper .site {
  background-color: aqua;
  border-bottom: 1px solid #fff;
  height: 40px;
  line-height: 40px;
}
```

## 230911

### 1. 넘치는 컨텐츠 제어 overflow

- 스크롤바 표시 여부 결정
    - `overflow: visible;` 기본값. 한정된 영역에서 컨텐츠가 넘치면 보여짐.
    - `overflow: hidden;` 한정된 영역에서 컨텐츠가 넘치면  숨김.
    - `overflow: auto;` 한정된 영역에서 컨텐츠가 넘치면 자동으로 스크롤 생성
    - `overflow: scroll;` 한정된 영역에서 무조건 스크롤이 생김.
    - `overflow: inherit;` 상속. 상속은 현재 부모나 조상 요소에 overflow가 적용된 게 없으면 상속 받지 못함.
- overflow X축 컨트롤

```
.box {
  overflow-y: hidden; /* 1. 일단 y축 없애줌 */

  /* 2. 글자의 띄어쓰기 기준으로 줄바꿈 처리 */
  white-space: wrap; /* 기본값. */
  white-space: nowrap; /* br요소로 직접 줄바꿈 시키는 것 외엔 자동 줄바꿈 되지 않음 */
}
- overflow Y축 컨트롤
  overflow-y: scroll; /* 무조건 스크롤 */
  overflow-y: hidden; /* 넘치면 숨기기 */
  overflow-y: auto; /* 넘치면 스크롤 */
}
```

### 3. 요소 성격 변경 display+visibility+opacity

- `display` 블록 레벨 요소를 인라인 요소로 바꾸거나 인라인 레벨 요소를 블록 레벨 요소로 바꿀 수 있다.
    - `inline` 요소의 기본 성격 변경. 상속x. 해당 요소에만 적용
    - `block` 인라인요소를 블럭요소로 변경.
    - `inline-block`
        - 인라인, 블록 성격 모두 가짐
            - 인라인처럼 띄어쓰기, 줄바꿈 인식
            - 인라인처럼 line-height 값을 가짐
            - 블록처럼 width, height 값을 가짐
            - 가로 중앙 정렬의 경우 인라인, 블록 적용 방식 다 가능.
            - 다만, 띄어쓰기가 있어 인라인 방식으로 정렬하는 것이 좀 더 편함.
    - `none` 브라우저 영역에서 사라짐. 코드 창에서만 확인 가능하며 레이아웃에 영향을 줌.
- `visibility: hidden;` 브라우저 영역은 남으나 컨텐츠가 보이지 않음. visible=보임, hidden=숨김
- `opacity`: 불투명도 조절. 자식에게까지 영향을 줌. 0~1사이 값

## 230912

### 박스 모델: 요소의 실제 크기 계산법

- box-sizing: content-box;/* 기본값 width+margin+padding+border
- box-sizing: border-box;/* width(padding+border)+margin

### 어절 기준 줄바꿈 제어 (띄어쓰기 기준)

- `word-break: normal;` 기본값.
- `word-break: break-all;` 어절에 맞춰 줄바꿈. 단, 영어 한정.
- `word-break: keep-all;` 어절을 유지하며 줄바꿈. 한글에 적합.

## 230913

### 1. 리스트 스타일 축약형

- ul 스타일을 변경.
- `ul` 혹은  `li`에도 사용 가능.

```
ul {
  width: 300px;
  /* 잘 사용하진 않음.
      list-style-type: lower-greek;
      list-style-position: inside;
       */
  list-style: inside square; /* 축약형. 띄어쓰기로 구분. */
  list-style: none; /* 주로 메뉴를 만들 때 사용. 가장 많이 사용. */
}
```

### 2. 테이블 스타일

- table은 자신만의 고정값이 있어서 부모에게 상속받지 못한다.
- table 태그에 border태그로 테두리를 줄 경우 기본으로 중앙 정렬이 된다.
- 페이지에서 중앙정렬 →  width값 없이 마진값으로만 적용.
- 셀과 셀 사이의 간격. 테이블 요소에만 적용되는 전용 속성.
    - `border-spacing: 0px;`
    - `border-spacing: 0px 0px;` /_ X축 Y축 순으로 적용. _/
- 셀과 셀의 겹치는 셀 조정.
    - `border-spacing: 0;` 먼저 사이 간격 값 0으로 초기화.
    - `border-collapse: separate;` 기본값. 겹치는 셀 테두리 값 그대로 둠.
    - `border-collapse: collapse;` 겹치는 셀 테두리 값 제어
- 컨텐츠가 없는 경우 셀 처리 방법
    - `empty-cells: show;` 셀 남김. 기본값

## 230914

- 마우스를 올렸을 때 생기는 아웃라인을 없애기 위해서는 <outline: none;> 명령어를 쓴다
    - *크럼, 엣지, 웨일 등 모던 브라우저에서 생기는 현상으로 포커스 상태일 때 테두리를 없앰*
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/a669081c-5776-46fa-897c-e787e4b50139/db915c41-e272-47bc-aaca-57ba093be5a1/Untitled.png)
    

- input이 많을 경우에는 아래와 같이 type으로 구분해준다. /*속성 (특성) 선택자: 요소[속성], 요소[속성=값], [속성]*

```
form input[type="text"]:hover {
      background-color: aquamarine;
      border: 1px solid black;
```

- 마우스 커서 손가락 모양으로 바꾸기 <cursor: pointer;>

### 1. accent-color 속성

- `input`값에는 기본적인 color 스타일 적용이 안된다.
- input type=checkbox, radio, range, progress 컨트롤 값 제어. `accent-color: 색상;`

> https://caniuse.com/ →  내가 사용하려는 태그에 대해 브라우저에서 적용 되는지 확인 할 수 있다.
> 

### 2. :before :after

- 해당 요소로 작성한 내용은 드래그가 되지 않는다.
- 값으로 작성되는 부분은 텍스트 컨텐츠의 영역으로 코드값이 적용되지 않는다.
- `content` 생략 불가능. ""로 내용을 비워둘 순 있지만, 값은 절대 뺄 수없다. 무조건 작성.
    - `:before`, `::before`
        - 기준 요소 안의 컨텐츠 영역 앞쪽에 적용. 의사 요소
    - `:after`, `::after`
        - 기준 요소 안의 컨텐츠 영역 뒤쪽에 적용.

### 3. 단위 em

- 알파벳 M을 기준으로 만들어진 단위
- 부모의 `font-size`를 기준으로 값 설정
- 브라우저 기본 폰트 사이즈: 16px
- 1em = 16px, 2em = 32px
- '나'를 감싸고 있는 부모를 기준으로 설정.
- 브라우저마다 상대적인 값으로 표현.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/a669081c-5776-46fa-897c-e787e4b50139/a826f4fc-21b8-44e0-8e81-9984aab55f86/Untitled.png)

> http://pxtoem.com/ em=px 변환 사이트
> 

### 4. 단위 rem

- root, 즉 최상위 요소(html)의 font-size를 기준으로 설정

```
html {
  /* <- rem 기준. 최상위 root 요소 */
  font-size: 24px;
}
body {
  /* body는 html의 자식 요소. body 값에 font-size를 넣어도 rem에 적용되지 않는다. */
  font-size: 20px;
}
```

1. 단위 viewport
    - vw: viewport width, vh: viewport height
    - 뷰포트의 가로 세로 값을 기준으로 사용하는 상대 단위 값
    - 100분의 1 단위
    - 상대 단위인 %는 부모를 기준으로 값을 정하지만(부모 요소를 넘기지 않음),                                                                                                                vw vh는 부모와 상관없이 뷰포트를 기준으로 값을 정한다. (부모 요소를 넘김)
    - 스크롤 바 인식을 못하는 단점이 있다.

## 230915

**flex**

> `https://developer.mozilla.org/ko/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox`  개념 설명 1
> 

> [An Interactive Guide to Flexbox in CSS (joshwcomeau.com)](https://www.joshwcomeau.com/css/interactive-guide-to-flexbox/) 개념 설명 2
> 
- 기본은 row로 지정 되어있다.
- 박스를 아래로 붙일 때 1 → align-items: flex-end + height : 100vh
- 박스를 아래로 붙일 때 2 → align-self: flex-end (플렉스 아이템에 직접 적용

```css
/* margin: auto; center center */
/* margin-left: auto; 여백이 왼쪽으로 들어가기 때문에 아이템은 오른쪽 배치 */
/* margin-right: auto; 여백이 오른쪽으로 들어가기 때문에 아이템은 왼쪽 배치 */
/* margin-bottom: auto; 여백이 아래쪽으로 들어가기 때문에 아이템은 위쪽 배치 */
/* margin-top: auto; 여백이 위쪽으로 들어가기 때문에 아이템은 아래쪽 배치 */
```

## 230918

- 

## 230920

- box1 ~ ul li → box1을 제외한 box의 형제들 안에 있는 li에 명령
- *flex-item css 특성 종류 - order, flex-grow, flex-shrink, flex-basis, flex ...*
    
    ```css
    flex-grow: 0; 숫자가 클수록 더 큰 영역을 가짐. 가변값이 아니거나 0인 경우 적용되지 않음.
    flex-shrink: 1; 숫자가 클수록 더 큰 영역 감소. 가변값이 아니거나 0인 경우 적용되지 않음.
    flex-basis: auto; 기본 가로 값 설정. auto인 경우 width, height 등의 특성으로 가로 설정이 가능하나 단위값이 주어진 경우 설정 안됨.
    flex: 증가비율(flex-grow) 감소비율(flex-shrink) 기준비율(flex-basis);
    flex: 0 1 auto; 기본값
    ```
    
    - flex-order *: flex-item에 적용되는 속성으로 아이템 배치 순서 설정*
- flex-shrink 감소비율 →숫자가 클수록 감소 폭 커짐. 숫자가 클수록 아이템의 크기는 더 작아짐
    - flex-shrink: 1; → 기본값. 아이템이 컨테이너를 넘기지 않음
    - flex-shrink: 0; → *width의 값이 그대로 적용. 즉 넘치는 경우 컨테이너를 넘김*
- flex-grow 증가비율 →숫자가 클수록 증가 폭 커짐.
    - flex-grow: 0; → 기본값. 증가하지 않음
    - flex-grow: 1; 1:1:1:1 → 비율 값으로 동일하게 커져 컨테이너를 채움
- flex-basis 기준비율
    - flex-basis: auto; → 기본값. 아이템 컨텐츠 크기에 맞춰 grow 비율 설정
    - flex-basis: 0; → *플렉스 아이템의 컨텐츠를 제외한 영역을 기준으로 grow와 shrink 설정 (기준값 width 300 / grow:0 / shrink: 1)*
    - flex-basis: 300px; →*flex-shrink: 1; 적용되어 있어 컨테이너를 넘지 못함 (기준값 width 300 / grow:0 / shrink: 1)*

## 230921

### position

- position 요소의 배치
    - **static**
        - 기본값. 아무런 특성이 없기 때문에 주로 다른 포지션 값이 적용된 요소를 '초기화' 하고자 할 때 사용
    - **relative**
        - 일반적인 흐름에 따라 자기 자신을 기준으로 위치 지정. top, right, bottom, left 위치 특성과 함께 사용되거나 생략될 수 있음.
    - **absolute**
        - 일반적인 흐름에서 벗어나며 포지션이 적용된 가장 가까운 부모 요소를 기준으로 위치 지정. top, right, bottom, left 위치 특성과 함께 사용.
    - **fixed**
        - 일반적인 흐름에서 벗어나며 브라우저를 기준으로 위치 지정. top, right, bottom, left 위치 특성과 함께 사용. transform, perspective, filter 특성이 부모 요소에 적용되어 있으면 그 요소를 기준으로 삼음.
    - **sticky**
        - 일반적인 흐름을 가지나 top, right, bottom, left의 값에 따라 offset 적용(스크롤 이벤트)

## 231005

- ::before, ::after 사용 시 content 태그는 꼭 들어가야 한다. 다만 비워둬도 된다.(ex. content: “”;)
- overflow: hidden; → 마진 상쇄 현상을 없앨 수 있다.
- aspect-ratio: 1/1; → 가로, 세로 비율을 맞춰준다 (content가 넘지 않는 경우에만 사용 가능)
- 위에서 준 left 값을 무력화 시키기 위해서는 아래 left : auto; 값을 준다

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/a669081c-5776-46fa-897c-e787e4b50139/f9c05a82-df38-47e5-b9a8-fd2b2cb1e354/Untitled.png)

## 231011

### grid

> https://studiomeal.com/archives/533→ 그리드 참고 사이트
> 

```css
grid : row(행 )/ column(열)
    grid-container 속성 : grid-template, grid-area, gap, justify-content, align-item...
    grid-item 속성 : grid-row, grid-column, justify-self, aling-self...
```
