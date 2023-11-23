# The Web Developer 부트캠프 2023 - React
# 목차
- [섹션 60 : 리액트 소개](#섹션-60--리액트-소개)
    - [리액트 소개](#리액트-소개)
    - [JSX 개요](#jsx-개요)
    - [기본적인 리액트 앱 구조](#기본적인-리액트-앱-구조)
    - [첫 번째 리액트 컴포넌트 만들기](#첫-번째-리액트-컴포넌트-만들기)
# 섹션 60 : 리액트 소개
## 리액트 소개
- 컴포넌트를 정의해 사용자 인터페이스를 구축할 수 있게 도와주는 라이브러리
- 여러 개의 작은 모듈을 계층 구조로 결합해 나가 더 큰 사용자 인터페이스를 만들 수 있게 도와줌
### 컴포넌트
- 복잡한 프론트엔드를 작은 개별 모듈로 나눈 것
- JS 기능 및 로직 부분과 html, css와 같은 프레젠테이션 부분으로 결합됨
## JSX 개요
- 컴포넌트를 작동하는 방법 : 스스로 HTML을 랜더링 할 수 있는 Js 함수를 만드는 것
- 함수에서 반환 하는 것은 실제 HTML이 아님
- JSX(JavaScript Syntax Extension) : 자바스크립트 확장 문법
    - Js 파일 안에 HTML 콘텐츠를 추가할 수 있게 함
    - 바닐라 Js와 다르기 때문에 변환하는 과정이 필요
## 기본적인 리액트 앱 구조
- `App`이라는 컴포넌트가 있어야 함
    - 전체 애플리케이션의 최상위 컴포넌트
    - `App` 컴포넌트를 HTML 파일에 렌더링 함으로써, 하위 컴포넌트들 또한 같이 랜더링 됨
## 첫 번째 리액트 컴포넌트 만들기
```js
funciton Header() {
    return <h1>I'm a header camoponent!</h1>
}
function App() {
    <Header/>
}
```
- 컴포넌트 이름의 첫 글자는 대문자
- jsx를 return 함
- `App` 컴포넌트에 추가할려면 `<Header/>`와 같은 방식으로 추가 해야 함
# 섹션 61: JSX 세부 사항
## 컴포넌트 가져오기
- 보통 리액트 애플리케이션을 만들 때는 한 파일에 한 개의 컴포넌트를 넣음
- import, export를 사용하여 파일들을 연결해줌
```js
// Greeter.js
export default function Greeter() {
    return <h1>HELLO!</h1>
  }

// App.js
import Greeter from "./Greeter"
...
```
- export를 할 때 deafult를 써서 내보내는 게 일반적
    - import, export를 할 때 이름이 같을 필요 없음
    - export는 Dog로, import는 Doggy로 해도 됨
    - but, 잘 쓰이지 않음 -> 혼란스럽기 때문에
- {}를 활용하여 여러 개의 요소를 내보낼 수도 있음
    - {}를 활용할 때는 import와 export 하는 것의 이름이 같아야함
- ex) `export {Dog}`, `import {Dog} from "./Dog.js`
## JSX 규칙
- `<img>`, `<br>`, `<input>`과 같이 닫는 태그가 필요없는 태그들도 닫는 태그를 명시해야 함
    - ex) `<br/>`, `<input type='password'/>`
- 컴포넌트는 하나의 요소, 하나의 상위 요소만 반환해야 함
    - 한 컴포넌트가 두 개의 `<input>`을 반환할 수는 없지 만, 두 개를 묶은 `<div>`는 반환할 수 있음
- 요소들을 return할 때 괄호로 감싸면 HTML처럼 들여쓰기하여 보낼 수 있음
``` js
export default function LoginFrom() {
  return (
    <div>
      <input type="text" />
      <input type="password" />
    </div>
  );
}
```
## 리액트 프래그먼트
- 