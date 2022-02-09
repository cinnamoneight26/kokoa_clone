# kokoa_clone

Nomad coders 코코아톡 클론 코딩 강의 repository

`2022.02.02 ~`

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
