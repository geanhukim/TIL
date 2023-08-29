# The Web Developer 부트캠프 2023 - HTML/CSS
# 목차
- [섹션 3: HTML: 기초](#섹션-3-html-기초)
    - [HTML 개요](#HTML-개요)
    - [단락 요소](#단락-요소)
    - [제목 요소](#제목-요소)
    - [HTML 상용구](#html-상용구)
    - [목록 요소](#목록-요소)
    - [앵커 태그](#앵커-태그)
    - [이미지](#이미지)
    - [주석](#주석)
- [섹션 4 : HTML: 시맨틱(Semantics)](#섹션-4-html-시멘틱semantics)
    - [HTML5가 정확히 무엇인가?](#html5가-정확히-무엇인가)
    - [블록 vs 인라인 요소 - Div와 Span](#블록-vs-인라인-요소---div와-span)
    - [기타 요소 모음 - HR, BR, Sup, Sub](#기타-요소-모음---hr-br-sup-sub)
    - [엔티티 코드](#엔티티-코드)
    - [시맨틱 마크업 개요](#시맨틱-마크업-개요)
    - [시맨틱 요소 사용법](#시맨틱-요소-사용법)
    - [VSCode 팁: 에밋](#vscode-팁--에밋)
- [섹션 5: HTML: 폼과 테이블](#섹션-5-html-폼과-테이블)
    - [테이블: TR, TD, Th 요소](#테이블-tr-td-th-요소)
    - [테이블: Thead, Tbody, Tfoot 요소](#테이블-thead-tbody-tfoot-요소)
    - [테이블:Colspan & Rowspan](#테이블-colspan--rowspan)
    - [폼(Form) 요소](#폼form-요소)
    - [일반적인 입력 형식](#일반적인-입력-형식)
    - [가장 중요한 레이블](#가장-중요한-레이블)
    - [HTML 버튼](#html-버튼)
    - [이름 속성](#이름-속성)
    - [라디오 버튼, 체크박스와 선택창](#라디오-버튼-체크박스와-선택창)
    - [범위 및 텍스트 영역](#범위-및-텍스트-영역)
    - [HTML5 폼의 유효성 검사](#html5-폼의-유효성-검사)
- [섹션 6: CSS: 기초](#섹션-6-css-기초)
    - [CSS란?](#css란)
    - [스타일을 올바르게 담기](#스타일을-올바르게-담기)
    - [색 및 배경색 속성](#색-및-배경색-속성)
    - [색상 시스템: RGB와 알려진 색상](#색상-시스템-16진법)
    - [색상 시스템: 16진법](#색상-시스템-16진법)
    - [일반 텍스트 속성](#일반-텍스트-속성)
    - [픽셀로 글꼴 크기 지정하기](#픽셀로-글꼴-크기-지정하기)
    - [글꼴 집합](#글꼴-집합)
- [섹션 7: CSS: 선택자의 세계](#섹션-7-css-선택자의-세계)
    - [전체 요소 선택자](#전체-요소-선택자)
    - [ID 선택자](#id-선택자)
    - [클래스 선택자](#클래스-선택자)
    - [자손 선택자](#자손-선택자)
    - [인접 선택자와 직계 자손 선택자](#인접-선택자와-직계-자손-선택자)
    - [속성 선택자](#속성-선택자)
    - [유사 클래스](#유사클래스)
    - [유사 요소](#유사요소)
    - [계단식 CSS](#계단식-css)
    - [우선순위 CSS](#우선순위-css)
    - [인라인 스타일과 중요도](#인라인-스타일과-중요도)
    - [상속 CSS](#상속-css)
- 섹션 8: CSS: CSS 박스 모델
- 섹션 9: CSS: 유용한 CSS 속성들
- 섹션 10: CSS: 반응형 CSS 및 Flexbox
- 섹션 12 CSS 프레임워크 : 부트스트랩(Bootstrap)

# 섹션 3: HTML: 기초
## HTML 개요
- 마크업 언어(not 프로그래밍 언어)
- 웹 페이지라는 문서에 마크업을 하기 위한 언어 또는 구문
- HTML 요소(Elements) 
    - HTML를 작성하기 위해 필요함
- HTML 태그(Tag)
    - `<p>I am a paragraph</p>`
    - 위 와 같이 텍스트를 태그로 감싸는 것
## 단락 요소
- `<p></p>`
    - 태그 안에 있는 내용을 한 단락으로 묶음
    - 단락들 사이에 공간을 추가함
## 제목 요소
- `<h1 ~ 6></h1 ~ 6>`
    - 숫자가 높아질수록 크기가 줄어듦
    - h1 태그는 한 페이지에 하나만 존재해야 함
    - 상위 h 태그가 없다면 하위 h 태그는 존재할 수 없음
## HTML 상용구
   ```html
    <!DOCTYPE html>
    <html>
        <head>
            <title></title>
        </head>
        <body>
        </body>
    </html>
```
- `<!DOCTYPE html>`
    - HTML5를 사용하고 있다는 표식
- `<html></html>`
    - 문서의 최상위 요소
    - 모든 내용들은 `<html>`안에 있어야 함
- `<head></head>`
    - 메타 데이터 요소
    - 페이지 상에 보이지 않는 내용을 담음
- `<title></title>`
    - 브라우저 탭 상에 표시되는 정보
- `<body></body>`
    - 문서의 모든 내용을 담고 있는 요소
## 목록 요소
- `<ol></ol>`
    - 순서가 있는 목록
> <ol><li>a</li><li>b</li><li>c</li></ol>
- `<ul></ul>`
    - 순서가 없는 목록
> <ul><li>a</li><li>b</li><li>c</li></ul>
- `<li></li>`
    - 목록의 요소들을 묶는 태그
## 앵커 태그
- `<a href=''></a>`
- 하이퍼링크를 만드는데 사용
- href
    - 연결할 문서, 페이지, 웹사이트 등의 주소를 입력해줘야 함
- 속성(attribute) : 태그에 부여할 수 있는 정보
- 인라인 태그
## 이미지
- `<img src="" alt="">
`
- 닫는 태그가 없음
- src
    - 이미지의 주소를 입력해야 함
- alt
    - 이미지를 불러들이지 못했을 때에 대한 설명
## 주석
- `<!-- -->`
- 브라우저에 보이지 않는 내용
# 섹션 4: HTML: 시멘틱(Semantics)
## HTML5가 정확히 무엇인가?
- HTML을 정의하는 가장 최근의 표준
- 우리가 직접 업그레이드 하는 것이 아닌, 브라우저가 받아들이는 작동 방식
## 블록 vs 인라인 요소 - Div와 Span
> <span>inline</span><span>inline</span><div>div</div><div>div</div>
``` html
<span>inline</span><span>inline</span><div>div</div><div>div</div>
```
- 인라인 요소
    - 한 줄에 같이 위치함
- 블록
    - 한 줄을 다 차지함
- 제네릭 요소
    - 여러 콘텐츠를 하나의 그룹으로 설정함
    - 그룹으로 묶어 스타일을 적용하기 위해 사용 
    - `<span></span>`
        - 인라인 요소
    - `<div></div>`
        - 블록 요소
## 기타 요소 모음 - HR, BR, Sup, Sub
- `<hr>`
    - 닫는 태그 없음
    - 스크린을 수평으로 나눔
    > <hr>
- `<br>`
    - 닫는 태그 없음
    - 줄바꿈
    > asdfasdf<br>asdfasdf
- `<sup></sup>`
    - 윗첨자
    - > a<sup>2</sup>
- `<sub></sub>`
    - 아랫첨자
    - > a<sub>2</sub>
## 엔티티 코드
- HTML 대신 쓸 수 있는 코드
- 부호나 기호처럼 html 파일 내에 작성하기 곤란한 것들을 타이핑할 때 사용
- `&#174;`
    > &#174;
## 시맨틱 마크업 개요
- Semantic : 의미와 관련된
- 그냥 `<div>`로만 만들어진 페이지는 무엇이 의미있는 것인지 알기 어려움
- `<header>`, `<nav>`, `<footer>`와 같은 시맨틱 코드를 사용하면?
    - naver와 같은 크롤러 프로그램이 더 쉽게 코드를 이해할 수 있음
    - 또한, 스크린 리더와 같은 장비를 사용하는 사용자가 페이지를 더 잘 이해할 수 있음
    - 다른 개발자들이 코드를 잘 이해할 수 있음
## 시맨틱 요소 사용법
- `<main>`
    - 문서의 주요 내용을 나타냄
    - 여러 페이지에서 반복되는 내용은 포함되지 않음
- `<nav>`
    - 내비게이션 링크
- `<section>`
    - 웹/애플리케이션의 독립적인 부분
- `<article>`
    - 문서 내의 독립적인 구성
- `<aside>`
    - 사이드바, 말풍선 등
- `<header>`
    - 보통 내용을 소개
    - 보통 내비게이션 바를 포함
- `<footer>`
    - 꼬리말
- `<time>`
    - 시간과 날짜를 의미
    - 인라인 요소
- `<figure>`
    - 독립적인 내용
    - 보통 캡션을 포함
## VSCODE 팁 : 에밋
- `>`
    - `main>nav>ul>li`
    ```html
    <main>
        <nav>
            <ul>
                <li></li>
            </ul>
        </nav>
    </main>
    ```
- `+`
    - `h1+h2+h3`
    ```html
    <h1></h1>
    <h2></h2>
    <h3></h3>
    ```
- `*`
    - `ul>li*4`
    ```html
    <ul>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
    </ul>
    ```

# 섹션 5: HTML: 폼과 테이블
## 테이블: TR, TD, Th 요소
- `<table></table>`
    - 테이블 데이터를 나타냄
    - 안에 다른 요소를 넣지 않으면 브라우저 상에 나타나지 않음
- `<td>`
    - 표 한에 있는 단일 셀
    - `<td>`만 사용하면 내용들이 모두 한 행에 표시됨
- `<tr>`
    - 표 안에 있는 셀들이 모인 행
- `th`
    - 헤더를 정의
## 테이블: Thead, Tbody, Tfoot 요소
- 표를 논리 섹션으로 분리할 뿐, 특별히 다른 일을 하지 않음
- 각각 이 부분이 표의 헤더다, 주요 내용이다, 꼬리말이다를 나타냄
## 테이블: Colspan & Rowspan
- 각각 몇 개의 열&행을 차지할지 나타냄
## 폼(Form) 요소
- `<form></form>`
    - 텍스트/비밀번호 입력란, 버튼, 체크박스 등 여러 개별 폼 컨트롤을 품는 컨테이너
    - `action` 속성을 사용하여 HTTP요청을 어디로 가는지 제어
## 일반적인 입력 형식
- `<input>`
    - 일반적으로 `<form>`을 컨트롤 하는데 사용
    - `type` 속성을 수정하여 다양한 `input` 형식을 만들 수 있음
    - `placeholder`
        - 입력란의 임시 텍스트를 지정하는 속성
        - `input`에 무언가 입력하기 전, 비어있을 때 표시될 내용
## 가장 중요한 레이블
- `<label>`
    - `input`과 직접적으로 연결됨
    - 레이블을 클릭하여 input에 직접 입력을 할 수도 있음
    - `label`과 `input`을 연결할려면 `id`와 `for` 속성이 필요함
- `id`
    - 한 페이지에서 id는 한개의 요소에만 사용될 수 있음
    - `id` 활용해 하나의 `input`에 하나의 `label`를 연결할 수 있음
- `for`
    - `label`의 속성으로 `id`를 입력하여 `input`과 연결함   

    - <label for="username">Enter a Username:</label><input id="username" type="text" placeholder="username">  
    ```html
            <label for="username">Enter a Username:</label>
            <input id="username" type="text" placeholder="username">    
    ```
## HTML 버튼
- `button`
    - `form`안에 버튼이 있다면 `action`의 주소로 `form`을 보냄
- `type` 속성
    - `submit`
        - 기본 기능
    - `button`
        - 단순히 브라우저상에서 버튼으로 기능함
## 이름 속성
- `name`
    - 서버가 찾으려는 값을 지정
## 라디오 버튼, 체크박스와 선택창
- `<input type="checkbox">`
    - <input type="checkbox" name="agree_tos" id="agree" checked> <label for="agree">I agree to everthing</label>
    ```html
        <input type="checkbox" name="agree_tos" id="agree" checked>
        <label for="agree">I agree to everthing</label>
    ```
- `<input type="radio">`
    - 체크박스와 비슷, but 그룹 중에서 단 하나만 선택할 수 있음
    - <label for="xs">XS</label><input type="radio" name="size" id="xs" value="xs"><label for="s">S</label><input type="radio" name="size" id="s" value="s"><label for="m">M</label><input type="radio" name="size" id="m" value="m">
    ```html
        <label for="xs">XS</label>
        <input type="radio" name="size" id="xs" value="xs">
        <label for="s">S</label>
        <input type="radio" name="size" id="s" value="s">
        <label for="m">M</label>
        <input type="radio" name="size" id="m" value="m">
    ```
    - 각각의 항목마다 value 값을 지정해줘야 함
        - 그러지 않으면 name의 값으로 HTTP 요청이 전송됨
- `<selcet>`
    - <select name="meal" id="meal">
        <option value="fish">Fish</option>
        <option value="veg" selected>Vegetarian</option>
        <option value="steak">Steak</option></select>

    ```html
        <select name="meal" id="meal">
            <option value="fish">Fish</option>
            <option value="veg" selected>Vegetarian</option>
            <option value="steak">Steak</option>
        </select>
    ```
## 범위 및 텍스트 영역
- `<input type="range">`
    - <label for="cheese">Amount of Cheese</label><input type="range" id="cheese" min="1" max="100" value="75" steps="5" name="cheese_level">
    ```html
        <label for="cheese">Amount of Cheese</label>
        <input type="range" id="cheese" min="1" max="100" value="75" steps="5" name="cheese_level">
    ```
- `<textarea>`
    - <label for="requests">Any Special Requests?</label><textarea name="requests" id="requests" cols="40" rows="10" laceholder="Type something here"></textarea>
    ```html
        <label for="requests">Any Special Requests?</label>
        <textarea name="requests" id="requests" cols="40" rows="10" placeholder="Type something here"></textarea>
    ```
## HTML5 폼의 유효성 검사
- 제한을 추가하거나, input 또는 데이터의 유효성을 확인하는 것
- `required`
    - 해당 `input`의 값이 없다면 submit을 못하게 함
- `minlength`, `maxlength`
    - `text` input의 최소길이와 최대길이를 정함
- 몇몇 `input type`은 내장된 유효성 검사를 가지고 있음
    - `email`
        - @와 그 뒤에 문자가 있는지 확인함
    - `url`
        - "http://"와 같은 형태를 가지는지 확인함
# 섹션 6: CSS: 기초
## CSS란?
- Cascading Style Sheets
- html를 시각적으로 나타내기 위해 사용
- CSS Rules
    ```css
        selector {
            property: value;
        }
    ```
## 스타일을 올바르게 담기
- Inline Styles
    - html 요소에 직접 스타일을 적용하는 방법
    - 재사용이 어렵기 때문에 많이 쓰이지 않음
- `<style>` 
    - `<head>`에 `<style>`요소를 활용하여 스타일을 적용하는 방법
    - 페이지별로 동일한 css를 적용하기 어려움
- 외부 스타일시트
    - CSS를 위한 별개의 파일을 만들고 html에 연결하는 방법
    - ```html
        <link rel="stylesheet" href="css파일 명">
        ```
## 색 및 배경색 속성
- color
    ```
    color : 색상;
    ```
    - 글자색을 변경함
- background-color
    ```
    background-color: 색상;
    ```
    - 배경색을 변경함
    - 블록 요소라면 컨테이너에서 사용 가능한 모든 요소의 색상을 변경함
## 색상 시스템: RGB와 알려진 색상
- Named Color
    - 미리 정해진 영어 색상명
    - 140가지
- RGB
    - 빨강, 녹색, 파랑을 섞어서 다양한 색깔을 나타내는 방법
    - 각 색들의 값은 0~255
    ```css
    color: rgb(173, 20 219);
    ```
## 색상 시스템: 16진법
- RGB를 16진법으로 표헌하는 것
- #0f5679
    - 2자리씩 빨강, 녹색, 파랑
## 일반 텍스트 속성
- `text-align`
    - 요소에 가로 정렬을 설정
    - left, center, right
    - 요소 전체를 움직이는 게 아닌, 요소 안의 내용에 한해 적용됨
- `font-weight`
    - 텍스트에서 주어진 부분의 굵기를 조정
    - normal, bold와 같이 단어/100, 200과 같은 수치로 value를 설정
- `text-decoration`
    - 텍스트를 꾸미는 선을 조정
    - 밑줄, 취소선, 윗줄 등등
    - 선의 색, 모양, 종류를 설정할 수 있음
    - <p style="text-decoration: orange underline wavy">hello</p>
    ```css
    p {
        text-decoration: orange underline wavy;
    }
    ```
    - `<a>`의 기본 밑줄을 제거하는데 주로 사용
        - `text-decoration: none;`
- `line-height`
    - 줄 간격의 길이를 지정함
    - 다양한 단위를 사용함
- `letter-spacing`
    - 글자 사이 간격을 지정
    - 다양한 단위를 사용함
## 픽셀로 글꼴 크기 지정하기
- `font-size`
    - 폰트 크기를 지정함
    - 다양한 단위를 사용
- `PX`
    - 절대 단위(최종 결과 크기)
        - 영향을 받지 않으면 최소한 한 페이지 내에서는 동일한 크기를 가짐
    - 디스플레이의 크기나 다른 요소에 따라 1px이 각각 달라질 수 있음
## 글꼴 집합
- `font-family`
    - 폰트를 변경할 때 사용
    - ','를 통해 백업 폰트를 설정할 수 있음
    - 폰트를 직접 고르거나, 폰트 패밀리를 지정
        - 폰트 패밀리 : 다양한 폰트를 모아놓은 집합
# 섹션 7: CSS 선택자의 세계
## 전체 요소 선택자
### 전체 선택자
- `*`
- 문서의 모든 요소를 선택
### 요소 선택자
- 지정한 태그의 스타일을 바꿈
- `,`를 이용하여 여러 개의 선택자를 지정할 수 있음
    - ex) h1, h2{}
## ID 선택자
- id앞에 `#`을 붙여 선택자로 사용
    - ex) #hi {}
- 하나의 아이디는 한 페이지에만 나와야 함
## 클래스 선택자
- ID와 달리 클래스는 여러 요소에 적용 가능
    - 종류가 다른 요소에도 사용 가능
- 클래스를 통해 요소들을 그룹화 해서 비슷하게 스타일링 가능
- 클래스 앞에 `.`을 붙여 사용
    - ex) .hi {}
## 자손 선택자
- 부모요소와 자손요소를 띄어쓰기로 연결함
    - ex) li a{}
    - `<li>`안에 있는 `<a>`에만 스타일이 적용됨
## 인접 선택자와 직계 자손 선택자
### 인접 선택자 `+`
- ex) h1 + p {}
- `<h1>` 다음에 있으면서 같은 단계에 있는 `<p>`를 선택
### 직계 자손 선택자 `>`
- ex) div > li {}
- `<div>` 바로 아래에 있는 `<li>`를 선택
- not 자손, 바로 "한 단계" 아래에 있는 태그만
## 속성 선택자
- ex) input[type="text"] {}
- `<input>`중에 타입이 `text`인 요소들만 스타일을 설정
- 여러 클래스 중 특정 태그의 클래스만 지정할 수도 있음
    - ex) seciont.tag {}
## 유사클래스
- 선택자 끝에 붙여 상태를 특정하는 키워드
- `:`로 시작
### hover
- 커서를 올려 두었을 때
### active
- 무언가가 현재 활성화 되있을 때
    - ex) 클릭했을 때
### nth-of-type
- n번째 요소에 스타일을 적용함
- ex) a:nth-of-type(3)
    - 3번쨰 요소에 스타일을 바꿈
- ex) a:nth-of-type(3n)
    - 3번쨰 요소마다 스타일을 바꿈
## 유사요소
- 선택된 요소에 특정 부분을 선택
### first-letter
- 선택된 요소의 첫 글자를 선택함
- `::`로 시작
### first-line
- 선택된 요소의 첫 줄을 선택
### selection
- 텍스트를 드래그 했을 때 사용됨
## 계단식 CSS
- 적용된 스타일의 순서가 중요함
- 가장 마지막에 작성된 스타일이 적용됨
- 가장 마지막에 작성된 스타일시트가 적용됨
## 우선순위 CSS
- 하나 이상의 스타일이 동일한 요소에 적용되거나, 적용될 수 있는 경우 충돌이 발생함
- 더 구체적인 선택자가 적용됨 -> 더 높은 특이도를 가진 선택자가 적용됨
- ID > 클래스 > 요소 
## 인라인 스타일과 중요도
- ID, 클래스, 요소보다 더 구체적임
- 되도록 지양해야 함
### !important
- 특성의 값 뒤에 `!important`를 입력하면 자동으로 최상의 특이도를 가짐
- ex) h1 {color: red !important}
## 상속 CSS
- 구체적인 특성을 지정하지 않은 하위 요소에 상위 항목의 특성이 적용됨
- 일부 요소는 상속받지 않도록 기본 설정 되어있음
    - 특성 값을 `inherit`로 설정하면 상위 항목의 특성을 상속 받음