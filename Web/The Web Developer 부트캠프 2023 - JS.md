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
- [섹션 17: JavaScript 배열](#섹션-17-javascript-배열)
    - [배열 개요](#배열-개요)
    - [배열 임의 접근](#배열-임의-접근)
    - [Push와 Pop 메서드](#push와-pop-메서드)
    - [Shift와 Unshift 메서드](#shift와-unshift-메서드)
    - [Concat, indexOf, includes, reverse 메서드](#concat-indexof-includes-reverse-메서드)
    - [Slice와 Splice 메서드](#slice와-splice-메서드)
    - [참조 타입과 동일성 테스트](#참조-타입과-동일성-테스트)
    - [배열 + Const](#배열--const)
    - [다차원 배열](#다차원-배열)
- [섹션 18: JavaScript 객체 리터럴 (Literals)](#섹션-18-javascript-객체-리터럴-literals)
    - [객체 리터럴 (Object Literals) 개요](#객체-리터럴-object-literals-개요)
    - [객체 리터럴 생성하기](#객체-리터럴-생성하기)
    - [객체 외부 데이터에 액세스하기](#객체-외부-데이터에-엑세스하기)
    - [객체 수정하기](#객체-수정하기)
    - [배열과 객체 네스트 구성하기](#배열과-객체-네스트-구성하기)
- [섹션 19: 루프의 구조](#섹션-19-루프의-구조)
    - [For 루프](#for-루프)
    - [무한 루프의 위험성](#무한-루프의-위험성)
    - [배열 루프](#배열-루프)
    - [중첩 루프](#중첩-루프)
    - [또다른 루프: While 루프](#또다른-루프-while-루프)
    - [정지/break 키워드](#정지break-키워드)
    - [For 루프의 유용함](#for-루프의-유용함)
    - [객체 루프](#객체-루프)
- [섹션 20: 함수란?](#섹션-20-함수란)
    - [함수 개요](#함수-개요)
    - [우리의 가장 첫 번째 함수](#우리의-가장-첫-번째-함수)
    - [인수 개요](#인수-개요)
    - [인수가 여러 개인 함수](#인수가-여러-개인-함수)
    - [반환 키워드](#반환-키워드)
- [섹션 21: 함수 레벨 업](#섹션-21-함수-레벨-업)
    - [함수 범위](#함수-범위)
    - [블록 범위](#블록-범위)
    - [렉시컬 범위](#렉시컬-범위)
    - [함수 표현식](#함수-표현식)
    - [고차 함수](#고차-함수)
    - [반환 함수](#반환-함수)
    - [메서드 정의하기](#메서드-정의하기)
    - ['this'라는 불가사의한 키워드](#this라는-불가사의한-키워드)
    - [Try/Catch 사용하기](#trycatch-사용하기)
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

# 섹션 17: JavaScript 배열
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
## Concat, indexOf, includes, reverse 메서드
### concat
- 배열 2개를 합쳐 새로운 배열을 반환함
    ```js
    let array1 = ['a', 'b'];
    let array2 = ['c', 'd'];
    let array3 = array1.concat(array2);
    array3;
    //['a', 'b', 'c', 'd'];
    ``` 
### indexOf
- 배열에 특정 값이 있으면 그 값의 인덱스 값을 반환함, 없으면 -1
    ```js
    array.indexOf('a'); //0
    array.indexOf('d'); //-1
    ```
### includes
- 배열이 특정 값을 포함하는 지 확인후 true/false를 반환
    ```js
    array1.includes('a'); //true
    array2.includes('a'); //false
    ```
### reverse
- 배열을 뒤집음
    ```js
    array3.reverse();
    // ['d,', 'c', 'b', 'a']
    ```
## Slice와 Splice 메서드
### slice([n, m])
- 배열의 일부를 복사
- n부터 m-1까지의 값을 복사
    ```js
    let color = ['red', 'yellow', 'orange', 'green', 'blue'];
    color.slice(2);
    // ['orange', 'green', 'blue']
    color.slice(1,4);
    // ['yellow', 'orange', 'green']
    color.slice(-2);
    // ['green', 'blue']
    ```
### splice
- 기존 요소들을 제거/대체하거나 새로운 요소를 추가함
    ```js
    const months = ['Jan', 'March', 'April', 'June'];
    months.splice(1, 0, 'Feb');
    // ["Jan", "Feb", "March", "April", "June"]

    months.splice(4, 1, 'May');
    // ["Jan",   "Feb", "March", "April", "May"]
    ```
### sort
- 배열을 정렬함
- 문자열로 변환 후, UTF-16 유닛 값을 비교 후 정렬
- 보통 함수를 사용하여 커스터마이징 함
## 참조 타입과 동일성 테스트
- 내용이 같은 배열이라도 `==`나 `===`로 비교했을 때 결과는 false
- 비교되는건 배열의 값이 아닌 메모리에서 참조되는 값
- 배열을 생성하면 이것은 메모리에서 생성되어 고유한 주소를 가짐
- ```js
    let array1 = [1,2];
    let array2 = array1;
    array1 === array2; //true
    // 같은 참조 주소를 공유하기 때문
    ```
## 배열 + Const
- 배열을 생성할 때 `const`를 사용가능
- `const`를 써도 배열의 콘텐츠를 바꿀 수 있음
- but, 새로운 배열의 참조 주소를 할당하는 것은 불가

## 다차원 배열
- 배열에 배열을 중첩하는 것
    ```js
    let array = [[1, 2, 3],
                [4, 5, 6],
                [7, 8, 9]
                ];
    array[0][1]; // 2
    array[1][1]; //5
    ```

# 섹션 18: JavaScript 객체 리터럴 (literals)
## 객체 리터럴 (Object Literals) 개요
- 프로퍼티(property)의 집합
    - 프로퍼티 : 키-값 쌍
- 인덱스 값이 아니라 키를 통해 데이터에 접근함
- 다양한 값을 넣을 수 있음
- 배열과 달리 순서가 없음
## 객체 리터럴 생성하기
- ```js
    let person = {
        firstName: 'Mick',
        lastName: 'Jagger',
        age: 23,
        marriage: true,
        child: ['Jane', 'Shawn']
    }; 
    ```
## 객체 외부 데이터에 엑세스하기
- 대괄호, 따옴표 사용
    ```js
    person["firstName"]; // "Mick"
    ```
- 점 사용
    ```js
    person.firstName; // "Mick"
    ```
- 객체에서 만드는 키는 문자열로 변환 됨
## 객체 수정하기
- 대괄호/점 사용법을 통해 기존 객체 값을 바꾸거나, 새로운 키-값 쌍을 추가할 수 있음
```js
person.age = 54;
person['age']; //54
person.['job']= 'doctor';
person.job; //'doctor'
```
## 배열과 객체 네스트 구성하기
- 배열 + 객체 리터럴
- 객체 안에 배열을 넣을 수도 있고, 배열 안에 객체를 넣을 수도 있음
# 섹션 19: 루프의 구조
## For 루프
- 같은 일을 반복할 때 동일한 코드를 여러 번 적는 대신 루프를 활용
- ex
    ```js
    for (let i = 1; i <=10; i++) {
        console.log(i);
    }
    ```
## 무한 루프의 위험성
- 멈추지 않는 루프
- 브라우저와 js의 메모리가 부족해 중단되긴 함
- 컴퓨터가 원하지 않는 방향으로 작동하거나, 브라우저가 잠길 수도 있음
- So, 어떤 시점에 루프가 정지할 것인지 확실히 해야 함
## 배열 루프
- 루프를 통해 인덱스 값을 늘려나가면서 배열에 접근할 수 있음
## 중첩 루프
- 루프 안에 있는 루프
- 루프1(i=0; i<=5)안에 루프2(j=0;j<=3)이 있다
    - 루프1이 한 바퀴 돌 때, 루프2는 세 바퀴 돔
    - 루프1이 두 바퀴 째일 때, 루프2는 다시 세 바퀴를 돔
## 또다른 루프: While 루프
- ex
    ```js
    let num = 0;
    while (num < 3) {
        console.log(num);
        num++;
    }
    /*
    0
    1
    2
    */
    ```
## 정지/break 키워드
- 특정 조건뒤에 `break`를 작성하면 크 조건을 만족한 뒤에 루프를 끝냄
## For 루프의 유용함
### for...of
- 반복 가능한 객체에 대해 객체의 원소에 변수명을 통하여 루프를 실행
```js
const array1 = ['a', 'b', 'c'];

for (const element of array1) {
  console.log(element);
}

/*
'a'
'b'
'c'
*/
```
## 객체 루프
- 객체 리터럴은 반복 가능한 객체가 아님
- for..of 문이 아닌 다른 방법을 써야 함
### for...in
- 객체 리터럴을 반복 함
- 잘 쓰이지 않음
### Object.keys/values/entries()
- 객체 리터럴의 키/값/키-값 배열을 가진 배열을 반환
# 섹션 20: 함수란?
## 함수 개요
- 코드의 재사용 가능한 일부를 언제든 사용할 수 있도록 이름을 붙여놓은 것
- 코드의 중복을 줄이고, 더 읽기 쉽게, 이해하기 쉽게 만들어 줌
## 우리의 가장 첫 번째 함수
- 함수 정의
    ```js
    function funcName() {
        code
    }
    ```
- 함수 실행
    ```js
    funcName();
    ```
## 인수 개요
- 함수에 입력하는 값
- 함수 정의 때 소괄호 안에 변수 이름을 넣어서 활용함 -> 매게변수
- 주어져야 할 인수가 전달되지 않으면 `undefined`가 전달됨
## 인수가 여러 개인 함수
- 인수를 넣을 때 쉼표를 통해 구분함
- 인수들을 활용할 때 순서가 중요함
## 반환 키워드
### return
- 함수의 결과 값을 변수에 저장할 수 있게 함
- `return`을 사용하면 함수가 종료됨
# 섹션 21: 함수 레벨 업
## 함수 범위
- 변수를 js 어느 부분에 정의하는냐가 엑세스 지점을 정의함
- 변수를 함수 밖/함수 안/함수 안의 중첩 함수 등등 다양한 곳에서 정의할 수 있음 -> 이것이 나중에 영향을 끼침
- 함수 안에서 `let`을 사용해서 만든 변수는 그 함수로 범위가 한정되어 있음
```js
function collectEggs() {
    let totalEggs = 6;
}
collectEggs();
console.log(totalEggs); //error
```
## 블록 범위
```js
let radius = 8;
if (radius > 0) {
    cons PI = 3.14159;
    let msg = "HIII!"
}

console.log(radius); //8
console.log(msg); //error
```
- 블록
    - 함수를 제외하고 중괄호가 있는 모든 곳 
        - ex) 조건문, 루프...
    - 블록 안에서 정의된 변수는 블록 밖에서 접근할 수 없음
- `var`로 변수를 지정하면 변수의 범위가 블록으로 지정되지 않음
## 렉시컬 범위
- 부모 함수의 안에 중첩된 내부 함수는 해당 외부 함수의 범위나 또는 범위 내에서 정의된 변수에 엑세스 할 수 있음
## 함수 표현식
```js
const add = function (x, y) {
    return x + y;
}
add(3, 4); //7
```
- 변수의 함수를 저장, 함수를 호출 할때 변수를 사용
## 고차 함수
- 다른 함수와 함께 작동하거나, 다른 함수에서 작동하는 함수
- 함수를 인수로 하여 다른 함수로 전달할 수 있음
    - 전달할 때 `함수()`가 아닌 `함수`로 전달해야 함
        - `함수()`일 경우 함수의 return 값이 인수로 전달 됨
## 반환 함수
- 함수 내에서 함수를 값으로 반환
## 메서드 정의하기
- 객체 리터럴에 함수를 정의
```js
const math = {
    multiply : function(x, y) {
        return x *y;
    },
    dvide(x, y) {
        return x / y;
    }
}
```
## 'this'라는 불가사의한 키워드
- 메서드가 정의하는 객체를 가르킬 때 사용
- 호출 컨텍스트에 따라 값이 달라짐
    - 객체 안에서 메서드가 호출하는 `this.특성`은 객체 내의 특성을 호출함
    - 객체 밖에서 변수에 메서드를 정의한 후, 메서드가 호출하는 `this.특성`은 기존의 객체가 아닌 `Window`객체를 호출함
## Try/Catch 사용하기
- js의 오류 및 예외를 처리
- `try`문 안에서 오류 및 예외가 발생할 경우 `catch`안에 있는 코드를 실행함
```js
try {
    hello.toUpperCase();
} catch {
    console.log("ERROR!!");
}
```
# 섹션 22: 콜백과 배열
## forEach 메서드
- 배열 안에 각각의 원소에 대해 함수와 코드를 한 번씩 실행
    ```js
    let number = [1, 2, 3];
    numbers.forEach(function (el) {
        console.log(el)
    })
    // 1, 2, 3
    ```
## Map 메서드
- 콜백 함수를 수령해서 배열의 요소당 1번씩 실행한 후 새로운 배열을 만듦
    ```js
    let number = [1, 2, 3];
    numbers.map(function (el) {
        return el * 2;
    })
    console.log(number)
    // 2, 4, 6
    ```
## 화살표 함수 개요