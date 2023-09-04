# The Web Developer 부트캠프 2023 - JS
# 목차
- [섹션 14: JavaScript 기초!](#섹션-14-javascript-기초)
    - [JavaScript가 놀라운 이유](#javascript가-놀라운-이유)
    - [기본 요소 및 콘솔](#기본-요소-및-콘슬)
    - [JavaScript 숫자(Number)](#javascript-숫자number)
    - [NaN은 또 뭘까?](#nan은-또-뭘까)
    - [변수와 Let](#변수와-let)
    - [변수 업데이트하기](#변수-업데이트하기)
    -[연산자 구현 설명: i++ vs ++i](#연산자-구현-설명-i-vs-i)
    - [Const와 Var](#const와-var)
    - [불리언(Booleans)](#불리언booleans)
    - [변수 명명과 규칙](#변수-명명과-규칙)
- [섹션 15: JavaScript 문자열(String)](#섹션-15-javascript-문자열string)
    - [문자열 개요](#문자열-개요)
    - [Indices와 Length](#indices와-length)
    - [문자열 규칙(String Methods)](#문자열-규칙string-methods)
    - [인수가 있는 문자열 규칙](#인수가-있는-문자열-규칙)
    - [엄청나게 유용한 문자열 템플릿](#엄청나게-유용한-문자열-템플릿)
    - [Undefined와 Null](#undefined와-null)
    - [난수와 Math 개체](#난수와-math-개체)
- [섹션 16: JavaScript 판단 내리기](#섹션-16-javascript-판단-내리기)
    - [비교 연산자](#비교-연산자)
    - [등식: 삼중 등호 vs 이중 등호](#등식-삼중-등호-vs-이중-등호)
    - [Console, Alert, Prompt코드](#console-alert-prompt코드)
    - [JavaScript 실행하기!](#javascript-실행하기)
    - [If 구문](#if-구문)
    - [Else-If 구문](#else-if-구문)
    - [Else 구문](#else-구문)
    - [Truthy 값과 Falsy 값](#truthy-값과-falsy-값)
    - [논리 함수 AND](#논리-함수-and)
    - [논리 함수 OR](#논리-함수-or)
    - [논리 함수 NOT](#논리-함수-not)
- 섹션 17: JavaScript 배열
- 섹션 18: JavaScript 객체 리터럴 (Literals)
- 섹션 19: 루프의 구조
- 섹션 20: 함수란?
- 섹션 21: 함수 레벨 업
- 섹션 22: 콜백과 배열
- 섹션 23: JavaScript의 최신 기능들
- 섹션 24: DOM이란?
- 섹션 25: 잃어버린 퍼즐 한 조각: DOM 이벤트
- 섹션 27: 비동기식 JavaScript
- 섹션 28: AJAX와 API
- 섹션 29: 프로토타입, 클래스, 그리고 OOP
# 섹션 14: JavaScript 기초!
## JavaScript가 놀라운 이유
- 웹 페이지의 동작을 담당
## 기본 요소 및 콘슬
### 원시 타입
- Number
- String
- Boolean
- Null
- Undefined
## JavaScript 숫자(Number)
- 숫자 타입이 한 개
    - 양수, 음수, 정수, 소수 모두 포함
- 기본 수학 연산자
    - `+`, `-`, `*`, `/`, `%`, `**`
## Nan은 또 뭘까?
- Not a Number
- 숫자로 간주하지만 숫자가 아닌 값
- ex) 0/0, 1 + NaN
## 변수와 Let
### 변수
- 값에 어떤 이름을 지정하고 그 값을 저장하여 다시 쓰거나 업데이트, 불러올 수 있음
- `let 변수명 = 값;`
    - ex) `let year = 1985;`
- 변수간의 연산을 값으로 가진 변수는, 연산된 변수가 업데이트되도 영향을 끼치지 못함
    - ``` javascript
        let a = 5;
        let b = 3;
        let c = a + b;
        c; // 8
        let b = 5;
        c; // 8
        ```
## 변수 업데이트하기
- `+=`, `-=`
    - ex) 
        ```javascript
        let a = 1;
        a += 2; // 3
        a -= 1; // 2
        ```
- `++`, `--`
    - ex) 
        ```javascript
        let a = 3;
        a ++; // 4
        a --; // 3
        ```
## 연산자 구현 설명: i++ vs ++i
### i++(후위 증가)
- 변수의 현재 값을 반환한 다음 1을 증가
### ++i(전위 증가)
- 변수의 값을 1증가시킨 다음, 증가한 값을 반환
## Const와 Var
### Const
- constant(상수)
- 일정한 값, 바뀌지 않음
- 변수를 초기화할 때 에러가 발생함
### Var
- 변수를 만드는 예전 방식
## 불리언(Booleans)
- `true` or `false`
- 변수간 변환이 자유로움
    - ex) Number 변수에 boolean을 저장할 수 있음
## 변수 명명과 규칙
- 공백 금지
- 숫자 시작 금지
- 카멜 케이스
    - 변수명으로 두 단어 이상을 써야 할 경우, 첫 단어를 제외한 각 단어의 첫 문자를 대문자로 씀
    - ex) let helloWorld = 2;
- 한 글자 변수는 자제
# 섹션 15: JavaScript 문자열(String)
## 문자열 개요
- 텍스트 정보
- 값을 큰/작은 따옴표로 묶어야 함
    - `let username = "hi"`
- 값에 공백이 들어갈 수 있음
## Indices와 Length
### Indices
- 문자열의 각 문자들은 인덱싱 되어 있음
- 0부터 시작함
- 뒤에서부터는 -1로 시작함
- ```javascript
    let a = "coding";
    a[0]; // c
    a[5]; // g
    a[56]; // undefined
    ```
### Length
- 문자열의 길이를 나타냄
- ```javascript
    let a = "coding";
    a.length // 6
    ```
- 문자열끼리 `+`하여 합칠 수 있음
## 문자열 규칙(String Methods)
- Methods
    - 개별 string이 사용할 수 있는 빌트인 action
### .toUpperCase()
- 문자열의 문자를 모두 대문자로 바꿈
- 원본은 그대로
- 반대 : .toLowerCase()
### .trim()
- 문자열의 처음과 끝에 오는 공백을 지움
- 원본은 그대로
## 인수가 있는 문자열 규칙
- 인수
    = 메서드로 전달되어서 메서드의 동작을 변경하는 입력 값
### .indexOf(searchValue[, fromIndex])
- 문자열에서 처음 나오는 searchValue의 인덱스 값을 반환, 없으면 -1을 반환
- fromIndex
    - 문자열에서 찾기 시작하는 위치
### .slice(beginIndex[, endIndex])
- 문자열의 일부를 추출하면서 새로운 문자열을 반환
- beginIndex부터 endIndex의 전까지의 문자열을 반환
### .replace(searchValue, newValue)
- searchValue을 newValue로 변환함
## 엄청나게 유용한 문자열 템플릿
- 문자열 안에 표현식을 내장할 수 있는 문자열들을 만들고, 해당 표현식은 평가된 후에 문자열로 바뀜
- `I counted ${3 + 4} sheep;` -> `I counted 7 sheep` 
- 문자열 템플릿은 따옴표가 아닌 백틱 기호(`)로 묶여야 함
## Undefined와 Null
### Undefined
- 정의되어야 할 값이 정의 되지 않음
- 보통 우리가 의도적으로 설정하지 않음
### Null
- 일부러 값을 지정하지 않음
- 의도적으로 값으로 설정하기도 함
## 난수와 Math 개체
- ```javascript
    Math.round(4.9) // 5
    Math.abs(-456) // 456
    Math.pow(2, 5) // 32
    Math.floor(3.9999) // 3
    Math.ceil(3.222) // 4
    ```
- Math.random()
    - 0부터 1사이의 랜덤한 값을 반환
# 섹션 16: JavaScript 판단 내리기
## 비교 연산자
- `>`, `<`, `>=`, `<=`
- true or false 반환
- Number 뿐 만 아니라 String간의 비교도 가능
    - 유니코드간의 비교
## 등식: 삼중 등호 vs 이중 등호
### `==`
- 두 값이 같은지 비교
- 타입은 고려하지 않음
- 두 값이 다른 타입이면 타입을 같게 만들어 비교
```javascript
    5 == 5; //true
    7 == '7'; //true
    0 == false; //true
    null == undefined; //true
```
### `===`
- 값과 타입 모두 비교
```javascript
    5 == 5; //true
    7 == '7'; //false
    0 == false; //false
    null == undefined; //false
```
### `!=`, `!==`
- 비동등 연산자
- 두 값이 다르면 true 같으면 false를 반환
- 타입 고려 x/ 고려 o
## Console, Alert, Prompt코드
### console.log()
- 인수를 콘슬에 출력
### alert()
- 인수를 팝업 창을 통해 출력
### prompt()
- 값을 입력할 수 있는 팝업 창을 출력
### parseInt()
- String인 인수를 Number로 변환함
## JavaScript 실행하기!
- js파일을 만들고 html파일에서 `<script>`를 통해 파일을 연결함
- `<script>`는 `<body>`바로 전에 위치해야 함
## If 구문
```js
if (조건) {
    '값이 true일 때 실행될 코드'
}
```
## Else-If 구문
```js
if (조건1) {
    '값이 true일 때 실행될 코드'
}
else if (조건2) {
    '값이 true일 때 실행될 코드'
}
```
- 조건2는 조건1이 false일 때만 실행됨
## Else 구문
```js
if (조건1) {
    '값이 true일 때 실행될 코드'
}
else if (조건2) {
    '값이 true일 때 실행될 코드'
}
else {
    '실행될 코드'
}
```
- else 구문은 모든 조건문이 false일 때만 실행됨
## Truthy 값과 Falsy 값
- boolean외에 다른 타입들도 각각 Truthy 값과 Falsy 값 중 하나를 가지고 있음
- falsy 값
    - false
    - 0
    - ""(empty string)
    - null
    - undefined
    - NaN
- 나머지 값들은 모두 truthy
- boolean이 아닌 값들이 boolean으로 변경되어야 한다면 truthy or falsy인지를 확인하여 true or false를 반환함
## 논리 함수 AND
- `&&`
```js
1 == 1 && 2 == 2 //true
1 == 1 && 2 == 3 //false
```
- 첫 식이 거짓이면 다른 식은 평가하지 않음
## 논리 함수 OR
- `||`
```js
1 == 1 || 2 == 2 //true
1 == 1 || 2 == 3 //true
```
- `&&`가 `||`보다 우선순위가 높음
## 논리 함수 NOT
- `!`
```js
!null //true
!( 0 === 0) //false
!(3 <= 4) //false
``` 

# JavaScript 배열
## 배열 개요
- 순서가 있는 값들의 집합
```js
//empty array
let array = [];

//array of strings
let array = ['hi', 'heel', 'oo'];

//array of numbers
let array = [2, 4, 1, 6];

//mixsed array
let array = [true, null, 2, 'hi']
```
## 배열 임의 접근
- 배열도 string과 마찬가지로 인덱싱이 되어있음
- 0부터 시작함
- string과는 다르게 접근한 배열의 값을 변경할 수 있음
    - string.length를 넘는 숫자를 인덱싱하면 사이에 있는 배열에는 empty가 입력됨
## Push와 Pop 메서드
### push(elementN)
- 배열 끝에 값(elementN)을 추가
- 배열의 새 length를 반환
### pop()
- 배열의 마지막 값을 제거
- 마지막 값을 반환
## Shift와 Unshift 메서드
### Shift()
- 배열의 첫 값을 제거
- 제거된 값을 반환
### Unshift(elementN)
- 배열의 앞쪽에 값(elementN)을 추가
- 배열의 새 length를 반환