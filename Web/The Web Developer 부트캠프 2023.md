# The Web Developer 부트캠프 2023
# 목차
- 섹션 3: HTML: 기초
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
## 시멘틱 마크업 개요
- Semantic : 의미와 관련된
- 그냥 `<div>`로만 만들어진 페이지는 무엇이 의미있는 것인지 알기 어려움
- `<header>`, `<nav>`, `<footer>`와 같은 시멘틱 코드를 사용하면?
    - naver와 같은 크롤러 프로그램이 더 쉽게 코드를 이해할 수 있음
    - 또한, 스크린 리더와 같은 장비를 사용하는 사용자가 페이지를 더 잘 이해할 수 있음
    - 다른 개발자들이 코드를 잘 이해할 수 있음
## 시멘틱 요소 사용법
- `<main>`
- `<nav>`
- `<section>`
- `<article>`
- `<aside>`
- `<header>`
- `<footer>`
- `<time>`
- `<figure>`