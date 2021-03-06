## 08.17.21

### ***github, codesandbox.io, w3schools\***

***HTML (Hyper Text Markup Language)\*** : "웹페이지 표시 언어"

- 웹페이지 구조 표시
- 웹페이지 콘텐츠 표시

> **client server model**: client - request -> server - response -> client (클라이언트와 서버 1:1 연결, 논리적구성)

> **front-end**: client에서 보여지는 부분

> **web browser**에 초점 - 서버에서 데이터를 받고, 소스코드 번역

> **해석/번역방식**: 컴파일링, 인터프리팅, 렌더링
>
> - **compiling**: C, C++, C#, JAVA, Python - 대표적인 compiler 언어들
> - **interpreting**: 
> - **rendering**: 모델을 실제처럼 보이도록 - **"HTML, CSS, JavaScript"**

***CSS (Cascading Style Sheets)\***

> **Cascade**: "폭포"
>
> - 적용순서가 위에서 아래로 차례대로 적용이 되지만, 맨 밑에 있는 내용이 최종반영된다.

> **공통화 작업** - 최대한 코드길이 줄이기

<br />

<br />

## 08.18.21

### ***codesandbox\***

- create sandbox -> static
- IDE

***HTML\***

> **HTML Elements**(요소)
>
> - Ancestor, Parent, Child, Descendant

> **HTML Attributes**(속성): 태그에 관련된 추가정보를 가지고 있는 것
>
> - All HTML elements can have **attributes**
> - Attributes provide **additional information** about elements
> - Attributes are always specified in **the start tag**
> - Attributes usually come in name/value pairs like: **name="value"**
> - react.js는 xml을 따르기 때문에 문법이 엄격함  *  `<hr>` -> `<hr />`:  empty elements는 이와 같이 표시

> **HTML Paragraphs**
>
> - p태그 사용시, 공백처리는 따로 공백태그를 사용하여 처리
>   - `<br>`
>   - ` `

>  **HTML Links**
>
> - 루트 상대 경로: 예를 들어, SSAC 건물 지하, 1층, 2층 각 층에 한명씩 있다고 가정하자. 그들에게 모두 3층으로 오라고 한다면 일단 모두 정문으로 가라고 한다 -> "/" - `"/"html/html_filepaths.asp`
> - id로 bookmark(책갈피)

> **HTML Lists**
>
> - 'u'nordered 'l'ist: `<ul>`
> - 'o'rdered 'l'ist: `<ol>`
> - 항목표시는 모두 'l'ist 'i'tems: `<li></li>`

>  **HTML Media**
>
> - video
>   - `controls` attribute: 재생버튼
>   - `autoplay muted` attributes: 크롬의 경우 muted 속성이 있어야 autoplay 
>   - `loop` attribute: 반복재생
> - image
>   - `alt` attribute: "alternative"

<br />

<br />

## 08.19.21

#### ***HTML\*** 

>  **HTML Semantics**
>
> - "Semantic": 의미의, 의미론적인
> - `<header>`, `<div>`, `<section>`, `<article>`, `<footer>`

> **HTML Block & Inline**
>
> - Block Elements: 다른 블럭요소, 인라인 요소 ,contents 모두 포함 가능
> - Inline Elements: 다른 인라인 요소, contents 포함 가능. 블럭 요소는 포함 불가.
>   - 예외: `<a>` - 인라인 요소지만 블럭요소도 포함 가능

> **HTML Entities**
>
> - HTML 마크업 용도로 fix된 기호는 대체 코드 사용

> **HTML id, class**



***CSS\***: Cascading Style Sheets

> **CSS Syntax**

> **CSS Selector**

<br />

<br />

## 08.23.21

***Review\***

> html semantics, border shorthand property, inherit

***CSS\***

> **Box Model**
>
> - width / height 기본 특성
>   - Block Elements: width는 parent elements에 맞춰서 채워짐, height는 child elements에 맞춰짐
>   - Inline Elements: width / height 적용되지 않음 => 레이아웃 구성 용도로 사용하지 않음
> - 단위
>   - px: px값으로 고정
>   - %: parent elements를 기준으로 특정 비율로 설정

***layout 구성 = "박스 배치" (flexbox)\***

> **배치**: 세로방향 배치, 가로방향 배치
>
> - 세로방향의 경우: 블럭요소의 기본성질이므로 굳이 설정 필요 X
> - 가로방향의 경우: legacy(X), float(X), Flexbox(O)

> **flexbox**
>
> - 당사자들한테 적용시키는 것이 아닌 부모요소에 적용(다른 박스 배치도 모두 부모요소에 적용)
> - `flex-direction`, 4가지 방향: column, row(default), column-reverse, row-reverse
> - reverse의 경우, 순서도 바뀌고, 정렬도 바뀜

> (pc -> mobile) "반응형 web"

> **justify-content**
>
> - `flex-start`(default), `flex-end`, center`
> - `space-around`: 각 박스의 왼쪽, 오른쪽에 동일한 여백
> - `space-between`: 첫번째 박스와 마지막 박스는 양쪽 끝으로 배치하고 그 사이 여백 동일하게

> **flex-wrap**
>
> - 원래 기본 flex는 웹페이지 크기에 따라 박스 크기가 설정됐음에도 불구하고 박스 크기를 줄이면서까지 무조건 가로로 배치
>
> - `flex-wrap: wrap;`은 설정된 박스 크기를 그대로 둔 상태에서 크기가 안맞는 박스들은 밑으로 내려서 배치
>
> - 부모의 영역으로 포함되지 않은 자식 영역이 밖으로 삐져나온다면?
>
>   -> 부모요소의 크기(너비, 높이)를 자식요소에 맞춰서 조절/명시(설정)

> **사진/영상 사이즈 조절**
>
> - **이미지**의 경우, 비율에 상관없이 가로/세로 설정하면 설정값에 맞게 변경. 그러나, **영상**의 경우, 비율이 저절로 맞춰지기 때문에 설정값에 상관없이 여백이 생길 수 밖에 없음.
>
>   -> 1. 위아래/양옆에 여백이 생기거나 
>
>   ```
>   2. 세로/가로 길이를 늘려서(전체 사이즈를 늘려서) 위아래/양옆 끝부분 안보이게
>   ```
>
>   -> width/height 둘 중 원하는 사이즈 하나만 설정하면 됨.
>
>   ex) 가로가 길고, 세로가 짧을 경우.
>
>   - 위아래 여백 생김. 박스 크기에 맞는 width, height 둘 다 설정하면, width는 맞춰지고, height는 위아래 여백이 생기고, 가운데(상하)로 맞춰짐.
>   - 여백을 없애고, height만 사용하여 높이를 맞출경우, 자식요소(비디오)가 부모요소(박스)를 넘어서 삐져나옴. -> 삐져나온 부분을 안보이게. => **"CSS overflow"**



***CSS overflow\***

> 부모요소 영역 < 자식요소 영역
>
> - `overflow`: `visible`(default) /  `hidden` /  `scroll` / `auto`
> - `auto`: 부모영역이 충분히 클 경우, 스크롤바가 보이지 않고, 부모영역이 자식요소보다 작게 되면, 스크롤바가 보이면서 스크롤 기능으로



***CSS RWD(Responsive Web Design)\***

> 반응형 웹 vs 적응형 웹
>
> - 반응형 웹: 하나의 사이트로 모바일용도 되고 pc용도 되는 웹, 모바일로 보나 pc로 보나 똑같음
> - 적응형 웹: 두개의 사이트(www. / m.)로 하나는 pc용, 다른 하나는 모바일용 웹

> Media Query
>
> - css 작성 시 `@media`는 가장 마지막에 작성 (remind: cascading)
> - 모바일까지 고려한다면, 해상도를 고려해야함. -> **"Breakpoint"** (desktop - tablet pc - phone)

> RWD Viewport
>
> - viewport를 안쓰면 pc화면을 축소해놓은 것처럼 보이지만, viewport를 쓰면 mobile화면이 pc와는 다르게 최적화되서 보임.



## 08.24.21

***Review\***

> **flexbox**
>
> - 부모요소에 높이가 정해져 있지 않을 때, 박스의 높이는 자식요소를 따라감. 부모요소에 높이를 명시해준다면 자식요소에 정해진 높이에 상관없이, 부모요소를 따름.
> - `align-items`(세로방향 배치)를 활용하면 부모요소의 높이에 상관없이 자식요소는 자식요소의 높이대로 세로방향으로 정렬된다. -> `flex-start`, `flex-end`, `center`
> - `align-content` -> `space-around`, `space-between`
> - "perfect centering": `justify-content: center; align-items: center;`
> - 총정리: `justify-content`- 가로방향 정렬, `align-items` - 세로방향 정렬.
>   - `flex-direction: column;`이라면, 90도로 회전 -> "가로가 세로, 세로가 가로"



***CSS display\***

> **display - inline / block**
>
> - 인라인요소는 박스가 제대로 적용이 안됨.
> - inline: 한 줄, block: 박스
> - `display: inline-block;` : 인라인 요소를 박스로 사용







***CSS Combinators\***

> 복합 선택자; 선택자 복수개 사용.
>
> - descendant selector (space)
>   - ex) `div p {}`: div에 포함된 모든 자손 p 적용
> - child selector (>)
>   - ex) `div > p {}`: div의 자식 p만 적용, 자손들은 적용 X



***CSS Pseudo-classes\***

> **가상 클래스**
>
> 1. 해당 요소의 상태구분, ex) `:active`, `:hover`, ...
> 2. 원하는 순서나 위치의 요소를 선택할때



***Git\***

> **git 기본 흐름**
>
> - 원격저장소(remote) 생성
> - 다운로드(clone)해서 로컬저장소(local)에 저장
> - working directory에서 작업하고 -> add(staging, "무대 위로 올린다")
> - add한 것들 commit하고 push(upload)



***JavaScript\***

> **Overview**
>
> - 프로그래밍 문법: 데이터, 명령구문, 함수, 객체, 클래스



***데이터 타입\***

> - 자바스크립트는 데이터 타입(숫자, 문자(열), boolean)을 구분하지 않는다.
> - 타입을 구분해서 사용해야 하는 경우 => **"TypeScript"**
> - JavaScript Booleans = True / False
>   - True != 0
>   - False = 0
> - Arrays, Objects: 데이터들을 묶어주는 방식



***variables\***

> - `const`를 사용하여 array를 만들었을 때, 요소 추가/변경은 가능하지만, 통으로 변경하는 것은 불가. 주소값을 다른 것으로 받는 것으로 인식



***operators\***

> - `===`: equal value and equal type
> - 비교할때는 항상 변수는 좌항에



***conditions\***

> - 조건문 => "분기문", ex) 로그인



## 08.25.21

***JS Switch\***

> **식(expression)에 따른 "분기"**
>
> - 분기되는 가지수가 많을 경우 if 구문보다 간편, case들을 나열
> - `if (condition)` vs `switch (expressino)`
>   - condition -> true / false
>   - expression -> 숫자나, 문자가 결과로 나오는 식 => "수식"
> - switch 구문은 if 구문으로 변경 가능
> - `break` 로 switch 구문 빠져나옴
> - 마지막에 `default`: 모든 case에 해당이 안된다면 수행
>   - if문에서 `else`와 같은 역할

***3항 연산\***

> **if구문과 유사**



***for loop\***

> ```
> for (statement1; statement2; statement3) {}
> ```
>
> - `statement1`: 최초 실행
> - `statement2`: 조건식
> - `statement3`: 반복하기 위한 변수 증감



***while loop\***

> ```
> while (condition) {}
> ```



***function\***

> **code block**
>
> - 함수 선언
> - 함수 확장
>   - 매개변수 사용
>   - `return` 사용

> **Arrow function**
>
> - 파이썬 람다와 비슷한 느낌
> - 코드길이 축소 가능 but 직관적이지 못함



***array\***

> - const
> - index



***object\***

> **"자동차"라는 객체(대상)**
>
> - 표기법: **camelCase**
> - property(속성)
>   - 자동차의 스펙
>   - 객체가 가지고 있는 정보들
>   - `object_name.property`
> - method(함수)
>   - 자동차의 기능
>   - 객체가 가지고 있는 기능들 => "함수"
>   - `object_name.method()`

> **accessing**
>
> - `objectName["propertyName"]`보다는 `objectName.propertyName`
> - `this.`: 객체 안에서 정의한 변수를 사용할때 앞에 붙임



***class\***

> - 표기법: **PascalCase**
> - "설계도", "대량생산이 가능"



***scope\***

> **변수의 범위**
>
> - global > function > block
> - 보다 포괄적인 범위에서의 변수만 보다 좁은 범위에서 사용 가능. 역은 불가.



***this keyword\***

> **this**를 포함하고 있는 **"객체"**를 가리킨다.





## 08.26.21

***JS HTML DOM\***

> **DOM (Document Object Model)**
>
> - tree구조로 html의 각각의 요소들을 객체화 -> JS로 각각의 요소들(객체들)을 control 가능

> **Accessing Element**
>
> - 동적생성(Dynamic): `document.getElementById("id_name").innerHTML = "Hello World"` - HTML에는 코딩을 하지 않고 JavaScript를 통해서 코딩(컨텐츠 생성)
> - 정적코딩(static): HTML 요소/태그에 직접 코딩



***script\***

> **defer (Attribute)**
>
> - 보통 script를 body전에 코딩하는데, 렌더링은 위에서 아래로 되기 때문에 적용이 안될 수도 있다. -> defer("미루다") 속성을 사용하여 위에서 코딩해도 렌더링될 수 있도록
> - external만 적용가능

> **DOM access**
>
> - `getElement(s)ById/ClassName/TagName`
> - `querySelector(All)`
>   - 무조건 하나에만 접근, 가장 가까운 것
>   - -> **querySelectorAll**로 가져오게 되면 객체로 가져옴

> **DOM 내용변경**
>
> - `createElement()`, `createTextNode()` `appendchild()`
>
>   - This code creates a new `<p>` element:
>
>     `const para = document.createElement("p");`
>
>   - To add text to the `<p>` element, you must create a text node first. This code creates a text node:
>
>     `const node = document.createTextNode("This is a new paragraph.");`
>
>   - Then you must append the text node to the `<p>` element:
>
>     `para.appendChild(node);`
>
>   - Finally you must append the new element to an existing element.
>
>   - This code finds an existing element:
>
>     `const element = document.getElementById("div1");`
>
>   - This code appends the new element to the existing element:
>
>     `element.appendChild(para);`
>
> - 내용추가를 하는데 너무 복잡함.
>
>   - 문자를 추가하기 복잡함
>   - `innerHTML`을 사용하면 기본에 있던 것들이 지워지고 새로 변경됨
>   - -> "jQuery"



***jQuery\***

> **$()** == $(document).ready() 
>
> - `script` tag에 `defer` attribute과 같은 역할
> - `$(Id/Class/Tag_Name).eq[indexNumber].append("<span>Hello World</span>")`
>
> **jQuery DOM** vs **JS DOM**
>
> ```
> - jquery DOM이 JS DOM보다 포괄적인 개념
> ```



***HTML Collection\*** vs ***NodeList\***

> **No Difference**



***AJAX\***

> **SPA (Single Page Application)**
>
> - 페이지 "전환"이 아니라, 하나의 페이지 내에서 "데이터만 변경"



## 08.27.21

***Node Control: 생성, 추가, 삭제, 변경\***

> **생성**
>
> - 동적 생성
>
> ```
> const elementName = document.createElement("element");
> const textName = document.createTextNode("text");
> elementName.appendChild(textName);
> ```
>
> - `const temp = element.appendChild("text");`
>   - 위와 같이, 변수에 저장 후 추가하게 되면, 화면에 출력되지 않는다.
>   - 화면에 출력을 원한다면, 변수에 저장하지 않고 명령만

> **추가**
>
> ```
> const domName = document.querySelector("class");
> domName.apendChild(elementName);
> ```

> **삭제**
>
> ```
> const listParent = document.getElementById("list");
> const removeChild = document.getElementById("remove-item");
> listParent.removeChild(removeChild);
> ```

> **변경**
>
> ```
> const changeNode = document.querySelectorAll(".list-item");
> console.log(changeNode);
> changeNode[0].innerHTML = "<span>text3</span>";
> ```



***Forms, CSS, Animations\***

> **DOM CSS**
>
> - 우선순위 고려
> - 원하는 이름의 class 추가
> - css를 직접 control하기보다는 class를 추가하여 control하는 것을 추천
> - `toggle()`: 왔다갔다 가능. ex)버튼을 누르면 생성됐다가 한번 더 누르면 사라짐

> **CSS 2D Transforms**
>
> - `transform` - attribute
> - `translate`/`rotate`/`scale`/`skew`/`matrix` - method(function)

> **CSS Animations**
>
> - @keyframe

> **CSS Transitions**
>
> - "motion(반응동작)" & "animation(자가동작)"
> - css에서 transition만 넣어주면 동작 가능
> - pc -> mobile
>   - 시작 상태 - - - - - - - Transition - - - - - - -> 끝 상태
>   - Transition: JavaScript로 제어



***HTML Input Types\***

> **Empty Elements**
>
> - `<input type="button">`: 태그로도 사용가능. 태그로 사용하는 것을 추천.
> - `<input type="checkbox">`
> - `<input type="password">`
> - `<input type="radio">`
> - ...
> - 프론트엔드 관점에서 볼 때, button의 경우, input보다는 본래의 태그 사용을 권장.



## 08.30.21

***Form Elements - Input, Select\***

> **Input types**
>
> - input tag에는 기본적으로 padding이 존재
> - `width: 100%` -> 부모요소에 너비 꽉 채우기
> - `box-sizing: border-box` ->  

> **addEventListener("change/input")**
>
> - change event: focus가 빠져야 작동
> - input event: 실시간으로 입력할때마다 작동
> - `addEventListener`: "입력된 값을 감지" -> "해당하는 동작 수행"
> - 매개변수를 사용하여 입력된 값(변수)을 바로 함수에 사용
> - `varName.currentTarget.value`: 입력한 값
> - `:focus` -> 마우스 커서 이동 시("focus 이동")  수행

> **Select**
>
> - `<option>`태그와 같이 사용. option에 `value=""` attribute을 추가하여 option값을 사용.
> - 연도 / 월 / 일 만들기
>   - 동적생성 -> `createElement()`,  `createTextNode()`, `appendChild()`
>   - for loop - DOM - 자식요소에 text 추가/생성 - attribute 추가/생성 - 부모요소에 text 추가/생성
>   - "일(날짜)"의 경우, 연도에 따라, 월에 따라서 다름 -> "연도, 월과 연결"
>     - `addEvenetListener` 활용
>   - 처음에 연도, 월 선택하면 일이 추가가 되는데, 다른 연도와 월로 바꿀 경우, `appendChild()`이기 때문에 전에 선택한 연도, 월에 해당하는 일이 그대로 남아있음.
>     - `innerHTML`을 활용하여 제거/변경
>     - 첫번째껀 그대로 두고, 날짜만 바꿀 순 없을까..? -> "퍼포먼스 향상



***Animation\***

> **sliding**
>
> - 오른쪽에서 왼쪽으로 - 오른쪽에서 화면에 들어오고 화면에 있던 미디어 왼쪽으로 나감 - 왼쪽에서 점프해서 다시 반복
>   - => 왼쪽으로 나가면 오른쪽으로 점프해서 들어오는 방식
> - "이동" => "좌표의 이동"
>   - CSS `position: aboluste` 사용
>   - 좌표는 부모요소를 기준으로
>     - 부모요소를 `position: relative`, 자식요소를 `position: absolute`로 설정
>     - 부모요소를 relative로 설정하지 않으면, 자식요소는 body 태그를 기준으로 움직임

> **advance_06.html**
>
> - 부모요소와 자식요소의 position을 설정하여 3장의 이미지를 겹쳐서 렌더링
>
>   - 겹쳐질 경우, 가장 밑 이미지가 맨 위에 보여짐
>   - 화면에 보여질 이미지를 제외하고는 이미지 모두 딱 붙어서 슬라이드
>   - 자식요소를 %로 쓸 경우, 부모요소를 px로 설정 필요
>
> - 애니메이션은 CSS로, 동작(롤링)은 JavaScript로
>
>   - CSS
>
>     - `left`: 100%에서 0으로 이동
>
>     - CSS로 상태를 3개로 나눔
>
>       - 나가기, 들어오기, 점프
>
>         - 점프는 굳이 필요없음
>
>           |          | state I    | state II   | state III  |
>           | -------- | ---------- | ---------- | ---------- |
>           | image_01 | in >>> out | out >>> -  | - >>> in   |
>           | image_02 | in         | in >>> out | out  >>> - |
>           | image_03 | -          | - >>> in   | in >>> out |
>
>   - JavaScript
>
>     - `setInterval()`: 무한반복(for loop는 시간의 개념 X)
>     - CSS에서의 시간은 애니메이션이 진행되는 시간. 즉, 이동하는 시간.
>     - JavaScript에서의 시간은 반복주기간격
>     - in, out, '' 에 인덱스넘버 0, 1, 2가 번갈아가면서 롤링
>     - 클래스를 각 인덱스에 추가해줌. 동시에, 기존 클래스를 제거해야 하는 클래스도 있음
>       - "모든 클래스를 다 먼저 지우고, 붙이고 싶은 인덱스번호에 붙인다."

> **play / pause**
>
> - play(default)
>   - 함수 선언
> - pause
>   - `clearInterval()`: 매개변수 사용
>     - `setInterval()`도 값이 나옴. 그 값을 매개변수로 사용하면 pause
> - play버튼을 여러번 누르면 이상하게 작동함 -> 처리 필요



***React\***

> **Node.js** 기반
>
> - 설치 / 버전확인
>   - terminal에서 `node --version`
> - npm 버전 확인
> - yarn 설치 / 버전 확인

> **Visual Studio Code**