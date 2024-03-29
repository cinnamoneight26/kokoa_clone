# kokoa_clone

Nomad coders 코코아톡 클론 코딩 강의 repository

`2022.02.02 ~`

-   CSS 선택자를 이전보다 정확하고 풍부하게 쓸 수 있게 되었음
-   :root를 사용할 수 있게 되었음
-   flex 사용에 익숙해졌음
-   position에 대한 이해도가 높아졌음
-   새로운 파비콘 등록방법을 알게 되었음
-   og, fb 등 새로운 메타태그를 알게 되었음
-   collapsing margin(여백 상쇄)에 대해 알게 되었음
-   BEM(Block Element Modifier)에 대해 알게 되었음
-   CSS의 flex children에서 order의 사용 방법에 대해 알게 되었음

---

### 2.0 Our First HTML File

### 2.1 설정 및 오류

    - 추천 확장 프로그램
      Waka Time
      Community material theme
      Material Icon Theme

    - 브라우저는 규칙을 따르지 않더라도 나에게 작성된 내용을 보여준다.
      HTML 파일에 에러가 있다고 말해주지 않으며 콘텐츠를 보여준다.
      이는 단점이자 장점.

### 2.2 첫 번째 HTML 태그

    - tag
      어디부터 어디까지의 구간이 tag인지 지정하는 도구
      태그를 닫아야 제대로 작동함

    - <h1> ~ <h6>

    - <h7>은 없으므로 작성하면 평범한 텍스트로 인식함

### 2.3 더 많은 태그와 더 예쁜

    - list
      <ol> ordered list : 순서가 있는 리스트(1, 2, 3...)
      <ul> unordered list : 순서가 없는 리스트

    - list item
      <li> list 안에 항목 만들 때 사용하는 태그

    - 추천 확장 프로그램
      Prettier : HTML 작성 시 닫는 태그가 없을 때 저장하면 자동으로 닫는 태그를 생성해 줌
      설치 - 좌하단 톱니바퀴 클릭 - Settings - 검색에 editor - format on Save 체크박스에 체크
      만약 그래도 적용이 되지 않는다면 format default가 다른 것으로 잡혀있을 수 있음
      cmd_shift+p -> Format Document width -> Prettier로 설정

### 2.4 태그 속성

    - a
      <a>는 anchor를 뜻함 (anchor : 닻)
      다른 웹사이트로 이동할 때 사용
      tag에 추가하는 부가적인 정보를 attribute(속성)이라고 함

    - href
      <a>태그를 사용할 때 쓰는 속성
      HTTP reference 혹은 hyperlink reference
      이동할 곳을 알려줌
      이 속성은 a 태그와 함께 쓸 떄 클릭할 수 있도록 함. h1에 href를 쓰면 클릭 및 이동되지 않음
      attribute href는 anchor 태그에서 작동함

    - target
      target attribute의 기본값은 _self
      _self : 해당 브라우저에서 링크 이동
      _blank : 새 탭으로 링크 이동

    - img
      img 태그는 다른 태그들과 다르게 /로 닫아주는 태그가 존재하지 않음
      img 태그는 self-closing tag (자체 닫기 태그)인데 img 태그 사이에 centent가 없는데, 이미지는 텍스트가 없기 떄문임

    - src
      img 태그가 쓰는 attribute
      scr는 img 태그의 contents라고 생각하면 됨

### 2.5 More Tags and head

    - img
    url을 이용하지 않고 local에서 가져온 img도 사용할 수 있음
    img에서 확장자와 위치는 정확하게 입력해주어야 함
    <img src="img/logo.jpg" /> 처럼 작성하는 것을 path notation(경로 표기법)이라고 함

    - HTML문서를 작성하는 규칙
    우리가 따라야 하는 형태가 있음
    HTML 문서는 항상 <!DOCTYPE html>로 시작해야 함
    이것은 브라우저에게 text파일이 아닌 html 문서라고 알려주는 것
    그 다음엔 <html> 태그를 열어주어야 함
    웹 사이트는 두 개의 파트로 나뉘어져 있음
    <html>태그 안에 <head>태그와 <body>태그를 넣어주어야 함
    <head>에서는 페이지와 관한 환경설정을 해주어야 함
    <title>태그는 <head>태그 안에서 사용함

### 2.6 All about the Head

    head에 있는 정보들은 검색 사이트에서도 사용됨
    구글에서 넷플릭스를 검색했을 때 나오는 문구는 title과 description
    meta tag의 meta는 부가적인 정보라는 뜻
    meta tag는 두 개의 attribute를 가지고 있음
    content와 name

    - <meta charset="utf-8">
    브라우저에게 text를 어떻게 그려달라는지 말해준다
    한글이나 다른 특수문자가 있는 언어를 입력할 때 사용함.

    - <html lang="">
    HTML에 lang을 지정하는 이유는 구글, 네이버 등 검색엔진들에 도움을 주기 위해서 작성함
    사이트에서 사용되는 언어가 무엇인지 말해주는 것

    - <link>
    rel(relationship)
    <link
            rel="shortcut icon"
            sizes="16x16 32x32 64x64"
            href="https://nomadcoders.co/m.png"
        />
    탭에 이미지 넣기. 파비콘이랑 다른건가? 신기함!!!!

    - og.image
      공유될 때 보여지는 이미지. 사이트 주소를 공유할 때 사용
      og:~ 네이버, 카카오톡....
      fb:~ 페이스북
      twitter:~ 트위터

### 2.7 More Tags

      - HTMl, CSS, JavaScript 등을 검색할 때 mdn 키워드 붙여서 검색하면 더 좋음
      (Mozilla devoloper Network)
      w3schools 사이트는 비추천

      - 단축키
      태그를 앞뒤 동시에 바꿔주는 거는 command + d

### 2.8 Form Tags

      - 기본적인 html 사용법
      <tagName attribute="attrValue"> contents </tagName>

      - form태그에는 수많은 attribute가 존재하지만 다 외울 필요 없음.
      필요할 때 검색해서 사용해도 됨.
      상술한 태그 사용법만 알면 언제든지 구현 가능!

### 2.9 More Tags and IDs

      - <label>
      form 태그 내에서 사용하는 태그
      레이블 태그는 for라는 attribute를 사용해서 input태그를 이용함
      input 태그의 id와 label의 for에 들어가는 값이 동일해야 함
      for와 같은 값을 가진 id를 들고 있는 input을 작동시켜 줌

      - id
      body 안의 어떤 태그에도 id를 넣을 수 있음
      id는 고유식별자임
      element당 하나의 id만 가질 수 있음
      scripting이나 css를 식별하려는 목적을 가지고 있음

      - 단축키
      커서 동시에 선택하고 싶을 때는 option(alt)키

### 2.10 Semantic HTML

      - <div>
      divison. 분할, 구분, 경계선
      시맨틱한 태그가 아님

      <header>
      시멘틱 태그.사이트의 헤더

      <main>
      시멘틱 태그. 사이트의 메인

      <footer>
      시멘틱 태그. 사이트의 꼬릿말

### 2.11 Recap

      HTML attribute에서는 항상 큰 따옴표 ""를 사용해준다.
      attribute를 작성할 때 ""를 잘 여닫아주어야 한다.
      특정 attrobute는 모든 태그에 사용할 수 있으며, 어떤 것은 특정 태그에만 쓸 수 있다.
      시멘틱 코드로 작성하는 것은 매우 중요하다.
      태그 암기하지 말 것. 필요할 때 검색해서 쓰는 게 효율적임.

### 3.0 How to Add CSS to HTML

      html문서에 css를 추가하는 여러가지 방법

      1. 같은 html파일에 html 코드와 css 코드를 놓는 방법
      2. css와 html을 분리s

      같은 html 파일에 css를 작성할 때 <style> 태그를 <head>태그에 포함시켜 인라인으로 사용

      분리해서 사용할 땐 css파일을 만들고 <link> 태그를 사용해 연결하여 사용
      작성시 href로 css를 연결해주고 rel로 html 파일과의 관계를 stylesheet라고 명시해줌

      둘 중 더 나은 방법은 1번처럼 분리된 파일을 만드는 것.

### 3.1 Writing Our First CSS Lines

      css 입력 규칙 3가지
      selector 지정
      속성이름에 띄어쓰기를 하지 않는다
      속성이름:속성값; 형태로 쓴다.

### 3.2 What Does Cascading Mean

      Cascading이 의미하는 바는 브라우저가 css코드를 읽을 때
      위에 있는 코드부터 차례대로 읽힌다는 뜻

      css 파일을 include하는 것을 external CCSS,
      HTML파일에 css를 작성하는 것을 inline CSS라고 함
      코드의 순서가 결과에 영향을 미침

      css는 위에서부터 아래로 읽히고 적용되는 것은 마지막 코드

### 3.3 Blocks and Inlines

      어떤 웹사이트든 그것을 이루는 모근 요소들은 box임
      box들로 디자인한다
      옆에 다른 요소가 못 오는 것을 block이라 부르고
      다른 요소가 올 수 있는 것을 inline이라고 함

      inline은 '같은 줄에 위치할 수 있다."
      (in the same line)는 뜻

      block은 옆에 아무 것도 올 수 없다는 것을 뜻함

      - inline 요소들
      아주 작은 글이나 링크, 그림 등등.
      inline애 해당하는 것은 많이 없기 때문에 block이 아닌 종류를 기억하는 것이 훨씬 편함
      <span>
      <a>
      <image>
      <code>

### 3.4 Margin Part One

      block을 inline으로, inline을 block으로 바꿀 수 있는데
      display 속성을 통해 변경이 가능함

      span의 display default값은 inline
      div의 display default값은 block

      inline요소는 높이와 너비를 가질 수 없기 때문에
      div에 inline을 주면 보이지 않음(div 안에 콘텐츠가 있으면 해당 내용은 보임)

      inline
            높이와 너비 없음

      block
            높이와 너비 있음
            margin, padding, border

      브라우저는 요소들에게 (원치 않아도) 많은 style 부여함
      크롬 개발자 도구에서 css에 user agent stylesheet로 보이는 것이
      브라우저가 기본적으로 지정한 style임

      margin은 box의 border(경계)의 바깥에 있는 공간

### 3.5 Margin Part Two

      margin을 방향없이 하나만 주면 상하좌우 모두 적용됨
      margin에 값을 두개 쓰면 상하, 좌우의 값 적용
      margin에 값을 네개 쓰면 위, 오른쪽, 아래, 왼쪽 값 적용(시계방향 순서)

      collapsing margin(여백 상쇄)
      https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing

      인접 형제 요소간의 margin은 서로 상쇄
      부모 블록에 border, padding, inline 부분이 없고 블록 서색 맥락이 생성되지 않았으면 상쇄된 여백은 부모 블록 바깥에 위치하게 됨
      테두리, 안쪽 여백, 인라인 콘텐츠, 높이, 최소 높이, 최고 높이가 없으면 블록의 마진이 상쇄됨

      강의에서는 부모의 경계와 자식의 경계가 같을 때 일어난다고 설명함

### 3.6 Paddings and IDs

      padding은 box의 경계로부터 안쪽에 있는 공간
      CSS에서 id를 명시할 때는 #뒤에 id를 쓰면 됨
      #id #first 등등..
      id="first"라는 의미가 됨

### 3.7 Border

      box의 경계
      border는 많은 속성을 가지고 있지만
      border에서는 여러 종류의 속성을 한번에 쓰진 않음
      이유는 정말 안 예쁨
      border: 2px solid black;
      너비, 스타일, 색깔 순서
      border-style: dotted; 이런 형태대로 쓸 수도 있음

      CSS에서 * 선택자는 전체를 뜻함
      inline도 border를 적용할 수 있을까?
      정답은 yes. border가 적용됨
      그렇다면 padding과 margin은 inline에 적용될까?
      inline에는 높이와 너비가 적용이 안 됨
      궁금한데 다음 시간에 알려준다고 함니다...

### 3.8 Classes

      inline요소에 padding을 주니 적용이 된다.
      margin은 사방에 줬는데 좌우에만 적용되고 상하에는 적용 안되는 것을 확인함
      inline은 padding은 다 가질 수 있지만 margin은 좌우로만 가질 수 있음
      inline은 모든 속성이 다 적용되지 않고 일부만 적용되는 경우가 있음

      css에서 요소를 여러개 지정하는 방법 #tomatoColor1, #tomatoColor2, #tomatoColor3 ...이런 식으로 쉼표(',')로 여러개를 나열해서 해결할 수 있음

      id처럼 요소를 지정할 수 있고 여러 요소를 한번에 지정하고 싶을 때는 class를 사용하면 됨
      .tomato는 class='tomato'라는 뜻과 같음
      클래스는 한번에 여러개를 적용할 수 있음

### 3.9 Inline Block

      div를 요소검사해보면 block으로 보여짐.
      이것은 브라우저가 지정한 것임
      block요소를 inline으로 변경할 수 있음
      display:inline을 css로 적용해주면됨

      inline-block은 inline을 block으로 인식하게 함
      inline-block으로 레이아웃을 할 수도 있지만 고루한 방식이고 여러 문제가 있음
      inline-block의 단점은 지정해주지도 않았는데 공간이 생긴다는 것과 정해진 형식이 없다는 것에 있음
      inline-block은 Responsive Design(반응형 디자인)을 지원하지 않음!!!!!
      그렇기 때문에 창크기가 달라지면 영향을 받음
      box를 나란히 두기 위해 inline-block을 사용하는 사람이 많지만 좋은 방법이 아님

### 3.10 Flexbox Part One

      inline-box의 문제점들이 발견되자 브라우저와 인터넷 커뮤니티에서 이를 고쳐보려함
      flexbox는 박스를 어떤 곳이든 둘 수 있고 아주 유연해서 2차원 레이아웃에서 아주 잘 작동함
      flexbox를 사용하기 위해서는 지켜줘야 할 중요한 규칙이 세 가지 있음

      1. 자식 엘리먼트에 어떤 것도 적지 말아야 한다. 부모 엘리먼트에만 명시해야함
            부모가 자식들을 제어하는 것임
            부모 엘리먼트에 display: flex;


      justify-content
            - 기본값은 flex-start
            - flex-start: 요소들을 컨테이너의 왼쪽으로 정렬합니다.
            - flex-end: 요소들을 컨테이너의 오른쪽으로 정렬합니다.
            - center: 요소들을 컨테이너의 가운데로 정렬합니다.
            - space-between: 요소들 사이에 동일한 간격을 둡니다.
            - space-around: 요소들 주위에 동일한 간격을 둡니다.

      align-items
            - flex-start: 요소들을 컨테이너의 꼭대기로 정렬합니다.
            -flex-end: 요소들을 컨테이너의 바닥으로 정렬합니다.
            - center: 요소들을 컨테이너의 세로선 상의 가운데로 정렬합니다.
            - baseline: 요소들을 컨테이너의 시작 위치에 정렬합니다.
            - stretch: 요소들을 컨테이너에 맞도록 늘립니다.

      flexboxfroggy : https://flexboxfroggy.com/#ko

      flexbox에는 주축(main axis)과 교차축(cross axis)이 있음
      주축은 수평이고 교차축은 수직임
      jestify-content는 주축에 적용되는 것임
      align-items라는 프로퍼티는 교차축에 적용
      align-items의 stretch는 요소를 늘어나게 하는데
      요소가 height값을 가지고 있으면 적용되지 않음

      vh
      viewport height.
      viewport는 screen이라는 말로 생각해도 됨
      100 screen height는 화면 높이의 100%를 의미함

      만약 부모 요소가 height를 가지고 있지 않다면 align-items을 설정하더라도 바뀌지 않을 것임. 이미 맨 위아래를 차지하고 중심에 있으니까.

### 3.11 Flexbox Part Two

      flex-direction
            - row: 요소들을 텍스트의 방향과 동일하게 정렬합니다.
            - row-reverse: 요소들을 텍스트의 반대 방향으로 정렬합니다.
            - column: 요소들을 위에서 아래로 정렬합니다.
            - column-reverse: 요소들을 아래에서 위로 정렬합니다.
            - column-reverse 또는 row-reverse를 사용하면 요소들의 start와 end의 순서도 뒤바뀝니다.

      order
            - flex 요소의 순서를 지정
            - -1, 0, 1 등 올 수 있으며 기본값은 0

      align-self
            - 지정된 alinge-items 값을 무시하고 flex요소를 세로선 상에서 정렬
            - flex-start
            - flex-end
            - center
            - baseline
            - stretch

      flex-wrap
            - nowrap: 모든 요소들을 한 줄에 정렬합니다.
            - wrap: 요소들을 여러 줄에 걸쳐 정렬합니다.
            - wrap-reverse: 요소들을 여러 줄에 걸쳐 반대로 정렬합니다.

      flex-flow
            - flex-direction과 flex-wrap이 자주 같이 사용되기 때문에 대신 사용함
            - 공백문자를 이용하여 두 속성의 값들을 인자로 받음
            - 예 : flex-flow: row wrap;

      align-content
            - 여러 줄들 사이의 간격을 지정
            - align-items는 컨테이너 안에서 어떻게 몯느 요소들이 정렬하는지를 지정
            - 한 줄만 있는 경우 align-content는 효과가 없음
            - flex-start: 여러 줄들을 컨테이너의 꼭대기에 정렬합니다.
            - flex-end: 여러 줄들을 컨테이너의 바닥에 정렬합니다.
            - center: 여러 줄들을 세로선 상의 가운데에 정렬합니다.
            - space-between: 여러 줄들 사이에 동일한 간격을 둡니다.
            - space-around: 여러 줄들 주위에 동일한 간격을 둡니다.
            - stretch: 여러 줄들을 컨테이너에 맞도록 늘립니다.

### 3.12 Fixed

      position
            - 레이아웃보다는 위치를 상하좌우로 옮기고 싶을 때 사용
            - top, bottom, left, right를 사용하지 않으면 초기 위치에 고정되고, 이들을 사용하면 형제 요소들과 다른 레이어를 사용하게 됨.
            - position:fixed를 사용하면 가장 위의 레이어에 머무름

### 3.13 Relative Absolute

      - position의 default값은 static
        레이아웃이 박스를 처음 위치하는 곳에 두는 것을 의미함

      - position : relative
        element가 처음 위치한 곳을 기준으로 수정

      - position : absolute
        가장 가까운 relative 부모를 기준으로 이동시켜 줌
        없으면 body가 기준이 됨

### 3.14 Pseudo Selectors part One

      기존에 배운 tag, id, class 선택자보다 조금 더 세부적으로 엘리먼트를 선택할 수 있음

      div:first-child
      div:last-child
      span:nth-child(even)
      span:nth-child(odd)
      span:nth-child(3n+1)
      span:nth-child(5n+1)
      .
      .
      .
      등이 있음

      HTML을 수정하지 않고 CSS만으로 손쉽게 선택하여 지정할 수 있음!

### 3.15 Combinators

      p span -> 이 방식으로 지정을 하면 p태그 아래의 span태그가 선택자가 됨
      p 안에서 span을 찾으라고 하는 것

      특정 부모 바로 아래에 있는 자식 요소를 셀렉터로 선택하고 싶으면
      div > span 방식을 사용하면 됨

      특정 요소의 형제 요소를 셀렉터로 선택하고 싶으면
      p + span 방식을 사용하면 됨 (next)

      정리
      p span : p태그 아래 모든 span 태그 지정
      p > span : p태그 바로 아래에 있는 span태그만 지정
      p + span : p태그와 같은 라인에 있는 형제 태그 중 span 태그를 선택. 바로 뒤에 있어야 선택됨. 중간에 다른 태그가 추가되는 경우 선택 해제됨

### 3.16 Pseudo Selectors part Two

      p ~ span
      span이 p의 현제인데 바로 뒤에 오지 않을 때 '~'를 사용함.

      input:required { border: 1px solid blue}
      input이 required라면 border 적용
      필수 입력값 표시할 때 유용할 듯

      input:optional { border: 1px solid blue}
      속성이 설정되지 않은 요소에 설정

      input[type="password"]
      input 요소 중 type이 password인 요소

      input[placeholder="username"]
      input 요소 중 placeholder가 username인 요소

      input[placeholder~="name"]
      input 요소 중 placeholder에 name이라는 단어를 포함한 요소

      https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors

### 3.17 States

      개발자 도구에서 확인할 수 있는 가장 중요한 selector

      :active : 버튼을 누르고 있을 때
      :focus : 키보드로 선택했을 때
      :hover : 마우스 커서가 대상 위에 있을 때
      :visited : 링크에만 적용. 방문한 적이 있는 링크 표시
      :focus within: 부모에 적용.
            focused인 자식을 가진 부모 엘리먼트의 상태를 말함

### 3.18 Recap

      ::placeholder
      placeholder를 스타일링 할 수 있게 해 줌

      ::selection
      텍스트를 selection했을 때 스타일링을 할 수 있게 함

      ::first-letter
      첫번째 글자의 스타일링을 할 수 있음

      ::first-line
      첫번째 줄의 스타일링을 할 수 있음

### 3.19 Colors and Variables

      CSS 컬러 시스템
      - hexadecimal color (16진수 컬러)
        #000000, #ffffff

      - RGB 방식
            rgba 방식도 사용할 수 있음
            여기서 a는 알파를 말하며 투명도를 뜻함

      - custom property (variable이라고도 함)

      :root
      기본적으로 모든 document에 뿌리가 됨
      변수처럼 사용할 수 있게함

      변수는 대쉬 2개 (--) 다음에 대쉬 1개, 그리고 변수이름
      빈 공간이 있으면 대쉬로 채워야 함.(빈 공간 허용하지 않음)

      :root {
                --main-color: #fcce00;
            }

      a {
                color: var(--main-color);
            }

### 4.0 Transitions

      어떤 상태에서 다른 상태로의 변화를 애니메이션으로 만드는 방법
      tranition은 state가 없는 요소에 사용해야 함
      먼저 어떤 것을 변화시킬지 쓰고 그 다음에는 얼마동안 변화가 일어나게할지 씀


      transition: all;
      변화하는 모든 것에 transition을 주는 것

### 4.1 Transitions part Two

      ease-in function
      브라우저에게 애니메이션이 어떻게 변할지 말해주는 것

      https://matthewlein.com/tools/ceaser

      디폴트로 가지고 있는 것.

      linear : 같은 속도로 좌우 직선으로 움직임
      ease-in : 시작점에서보다 빨라지며 움직임
      ease-in-out
      ease-out
      ease

      내가 속도를 직접 설정할수도 있음
      cubic-bezier(0,0,0,0)으로 직접 설정 가능

### 4.2 Transformations

      요소를 변형시키는 기술
      transformation은 box element를 변형시키지 않음
      margin, padding이 적용되지 않음
      일종의 3D transformation.
      CSS에 있는 모든 애니메이션은 GPU에 의해 돌아감
      컴퓨터 그래픽카드에 의해서 돌아감

### 4.3 Animations part One

      애니메이션을 만들기 위해서는 @keyframes 를 사용함

      @keyframes에는 두가지 옵션이 있음

             @keyframes coinFlip {
                from {
                    transform: rotateX(0deg);
                }
                to {
                    transform: rotateX(360deg);
                }
            }

            img {
                width: 300px;
                height: 300px;
                border: 5px solid black;
                border-radius: 50%;
                animation: coinFlip 5s ease-in-out;
            }

### 4.4 Animations part Two

      이런 방법도 씀
      원하는만큼 많은 스텝을 가질 수 있음
      예시는 3개

            @keyframes coinFlip {
                0% {
                    transform: rotateY(0deg);
                }
                50% {
                    transform: rotateY(180deg) translateX(100px);
                }
                100% {
                    transform: rotateY(0deg);
                }
            }

      반드시 transform을 사용해야하는 것은 아니지만 권장함.
      어떤 것은 애니메이션으로 잘 안되기 때문임.

### 4.5 Media Queries

      media query는 오직 CSS만을 이용해 스크린의 사이즈를 알 수 있도록 한다. (사용자가 보고있는 스크린)

            @media screen and (max-width: 600px) {
                div {
                    background-color: tomato;
                }
            }

            @media screen and (min-width: 601px) and (max-width: 1200px) {
                div {
                    background-color: wheat;
                }
            }

            @media screen and (min-width: 1200px) {
                div {
                    background-color: turquoise;
                }
            }

            @media screen and (orientation: landscape) {
                span {
                    display: none;
                }
            }

### 4.6 Media Queries Recap

      미디어 쿼리 사용

      https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries#media_features


      미디어 유형

      https://developer.mozilla.org/en-US/docs/Web/CSS/@media#media_types

      오직 휴대폰 디바이스에만 적용되는 미디어쿼리
      데스크톱 브라우저는 인식하지 못함
       -> min-device-width, max-device-width

      스크린이 레티나 디스플레이인지 아닌지 구분할 수 있음
      (아이폰, MacOS의 스크린)
       -> aspect-ratio

      프린트 css
       -> print

### 5.0 What is Git

      파일의 히스토리를 아는 것은 아주 중요한 일임
      GIT을 사용하면 파일을 무엇을 어떻게 작성했는지 변경 내역을 볼 수 있음
      text 파일 뿐 아니라 다른 파일의 변경 내역도 볼 수 있는데 git 시스템 파일은 binary format으로 인식하기 때문임.
      git은 파일을 계속 추적함 (Tracking)

### 5.1 What is Github

      Repository
      코드를 넣을 폴더라고 생각하면 쉬움
      코드의 변경 내역과 그 히스토리를 가지고 있는 폴더.
      public과 private를 선택할 수 있음
      commit은 기본적으로 시점이라고 생각하자.
      git은 파일들을 주시하면서 관리해주는 도구
      github는 git의 변경내역을 볼 수 있는 사이트

### 5.2 Creating a Github Repository

      Github Desktop 설치 후 온라인 repository를 로컬에 연결

### 5.3 Making Our First Commits

      1. 파일을 작성한 후 저장
      2. github desktop 좌측에 파일 확인
      3. 푸쉬할 파일에 체크박스 체크
      4. commit 타이틀 입력 후 commit
      5. push

### 6.0 Introduction

      .gitignore는 git 사용 시 업로드에 포함하고 싶지 않은
      파일 이름을 기록하는 파일
      (.DS_Store 추가해줌)

### 6.1 Sign Up Screen part One

      빈 html문서에 !치고 엔터 치면 기본 html 서식이 나온다.
      몰랐던 단축키
      니꼬쌤이 추천하는 id,class명 짓기
            -> 부모요소__자식요소(ex : status-ber__column)

### 6.2 BEM

      BEM : Block Element Modifier
      CSS 방법론 중 하나

      Block_Element--Modifier 방식으로 class네임을 명명함

      http://getbem.com/introduction/

### 6.3 Font Awesome

      아이콘을 추가하는 두 가지 옵션이 있음
      1. 직접 아이콘을 구하는 방법
      2. Heroicons(https://heroicons.com/) - 픽셀이 아닌 path로 되어 있는 이미지 아이콘,
         fontAwesome(https://fontawesome.com/) - 유료/무료 아이콘

      script는 항상 닫는 바디태그 ( </body> ) 직전에 두는 게 좋음

### 6.4 Sign Up Screen part Two

      로그인 페이지 마크업-

### 6.5 Status Bar CSS

      마크업에 유용한 단축키

      link:css
              <link rel="stylesheet" href="style.css">

      div.classname
              <div class="classname"></div>

      div#id
              <div id="id"></div>

      web font
      - link 보다 import를 추천한다.
      - import위치는 제일 상단
      - body에 font-family 추가
      - 모든 폰트를 추가하면 웹사이트 무거워진다.
        하나의 스타일을 선택한 것보다 불러오는데 시간이 오래 걸림. 사용하지 않을 폰트를 선택하지 않는 것도 중요
      [Google Fonts](https://fonts.google.com/)

      justify-content 대신 컨테이너 하나를 중심에 놓는
      css 기술
      .status-bar__column {
            width: 33.33333%;
      }
      .status-bar__column:nth-child(2) {
            display: flex;
            justify-content: center;
      }
      .status-bar__column:last-child {
            display: flex;
            justify-content: flex-end;
            align-items: center;
      }

### 6.6 Sign Up Screen part Three

      reset css

      https://cssdeck.com/blog/scripts/eric-meyer-reset-css/

      html에 link를 여러줄 만드는 것 보다 css에 import하여 사용하는 것이 나음

      크롬 확장 프로그램
      Page Ruler Redux extension

      웹페이지에서 드래그하여 px을 측정할 수 있음
      만약 작동이 안 되면 확장 프로그램 관리에 가서
      파일 URL 허용해줄 것

### 6.7 Log In Form part One

      로그인 페이지 form style

### 6.8 Log In Form part Two

      :not
      이것을 제외한 나머지에 적용하겠다는 css 선택자

      부모로부터 css 값을 상속받을 때 inherit를 사용
      #login-form a {
            text-align: center;
            text-decoration: none;
            color: inherit;
      }

### 6.9 Recap and Forms

      - form tag의 action은 어떤 페이지로 data를 전송할 것인지 지정할 수 있도록 함
      - action에 기재한 url에 해당하는 파일은 반드시 존재해야 함
      - method는 post 방식과 get방식이 있음
      - post방식은 백엔드 서버에 정보를 전송하는 방식.
      - get방식은 url에 정보를 추가하여 보내는 방식
      - get방식은 보안에 취약하므로 정보를 보낼 때는 사용하면 안 됨

### 6.10 Navigation Bar part One

      - navigation은 보통 ul로 나눠지고 그 안에 li로 구성됨

      - vscode 단축키
      nav>li>li*4>a

### 6.11 Navigation Bar part Two

      - 위치 고정을 위해서 position : fixed를 사용해야 함
      - 요소에 padding이 있을 경우 width: 100%일 때
      화면 밖으로 나가는 현상이 있을 수 있음
      그럴 때 사용하는 것이 box-sizing:border-box;

### 6.12 Border Box

      - 200px의 박스에 50px의 padding을 주면
      css는 기존 박스의 길이를 유지하기 위해 50px만큼 크기를 늘리기 때문에 내가 원하는 길이가 나오지 않고
      총 250px의 박스가 됨

      - box-sizing: border-box는 내가 지정한 박스의 크기를 유지한 상태로 padding을 사용할 수 있게 함

### 6.13 Navigation Bar part Three

      - friends.html bottom 마크업

### 6.14 Screen Header

      - friends.html header 마크업
      - header 부분은 공통으로 사용할 수 있기 때문에 컴퍼넌트화하여 구현

### 6.15 Friends Screen part One

      - friends.html name display 마크업

### 6.16 User Component part One

      - friends.html image, title 마크업

### 6.17 User Component part Two

      - friends.html Channel 마크업

### 6.18 Finishing Friends Screen

      - friends.html 마크업 마무리

### 6.19 Chats Screen part One

      - chats.html 마크업

### 6.20 Chats Screen part Two

      - chats.html 마크업
      - 공통으로 쓰이는 css에서 flex를 사용할 때
      영향을 피하고 싶은 html요소는 <div>로 감싸주면 해결.
      flex는 부모에 설정하고 자식에게 영향이 가기 때문에
      <div>로 감싸주면 영향을 피할 수 있음

### 6.21 Find Screen Part One

      - find.html 마크업
      - 숙제 : find 옆 아이콘에 붉은 색 도트 표시 만들기
      - 숙제 : chats.html에 margin-bottom 주기

### 6.22 Find Screen Part Two

      - find.html 마크업
      - 같은 코드가 계속 반복된다면 변수로 만드는 것이 좋음

### 6.23 Find Screen Part Three

      - find.html 마크업
      - 디자인을 위해 대문자를 사용하는 경우 css를 통해 가능
            ㄴ text-transform: uppercase;

### 6.24 Find Screen Part Four

      - find.html 마크업
      - justify-content: space-between; align-items: center;
        이 두 개는 함께 아주 자주 사용되는 CSS임

### #6.25 More Screen part One

      - more.html 마크업

### 6.26 More Screen part Two

      - more.html 마크업
      - settings.html 생성

### 6.27 Settings Screen part One

      - setting.html 마크업
      - header 영역 컴포넌트로 생성
      - herder css에서 column first-child에 margin-right를 auto, last-child에 margin-left를 auto로 주니 정렬이 예쁘게 됨

### 6.28 Settings and Chat Screen part One

      - chat.html 마크업

### 6.29 Chat Screen part Two

      - chat.html 마크업
      - .alt-header__column 부분 CSS - absolute를 이용해서
      정중앙에 오도록 하는 것은 부자연스러움.
      3개의 컬럼이므로 33%를 주고 정렬을 맞춰 가운데 오도록 수정
      어떤 요소를 고정하면 이전의 box들과는 다른 layer가 됨.
      - z-index : 숫자가 작을수록 낮은 layer, 클수록 위의 layer
            fixed absolute position에 이용가능

### 6.30 Chat Screen part Three

      - chat.html에서 타임스탬프 마크업
      - chat 수신 메세지 부분 마크업 진행 중

### 6.31 Chat Screen part Four

      - chat 수신 메세지 부분 마크업 진행

### 6.32 Chat Screen part Five

      - CSS의 order속성은 flex children에게만 적용된다.

### 6.33 Write Message Input

      - 채팅 입력창 부분 markup

### 6.34 Splash Screen part One

      - 페이지 새로고침 시 보여질 splash화면을 생성
      - 100vh는 화면 높이의 100%를 의미하고 100vw는 화면 넓이의 100%를 의미한다.

### 6.35 Splash Screen part Two

      - animation을 이용해 element 컨트롤 할 경우 디폴트값에 의해 다시 맨 처음 상태로 돌아옴
      - 위의 이유때문에 CSS의 anomation 끝에 forwards를 추가해준다. forwards는 마지막 속성값 (final property value)을 애니메이션이 끝나고 유지하도록 한다.
      - 예를들어 애니메이션에 지정한 마지막 속성이 opacity: 0이라면 애니메이션이 끝나고도 유지가 된다.
      - 하지만 이렇게 애니메이션을 통해 안 보이게 해도 element는 그대로 유지가 된 상태이기 때문에 요소 클릭이 진행되지 않는다.
      - 애니메이션의 마지막 속성에         visibility: hidden를 추가하여 요소를 숨김처리하면 문제 해결. visibility: hidden;은 요소가 마우스에 걸리지 않게 빠져버리는 상태.html의 요소는 아직 존재하는 상태. 무언가 숨긴다거나 할 때는 이 테크닉 사용은 권장하지 않음. 대체로 이런 경우 JavsScript를 이용하여 해결

### 6.36 Navigation Animation

      - CSS animation 진헹. from, to 외에 0%, 50%, 100% 등으로 구분하여 사용할 수 있음.
      - animation에 infinite를 사용하면 반복하여 움직임
