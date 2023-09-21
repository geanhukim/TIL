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
- [섹션 22: 콜백과 배열](#섹션-22-콜백과-배열)
    - [forEach 메서드](#foreach-메서드)
    - [Map 메서드](#map-메서드)
    - [화살표 함수 개요](#화살표-함수-개요)
    - [화살표 함수의 반환](#화살표-함수의-반환)
    - [setTimeout과 setInterval](#settimeout과-setinterval)
    - [Filter 메서드](#filter-메서드)
    - [Some과 every 메서드](#some과-every-메서드)
    - [악명 높은 Reduce 메서드](#악명-높은-reduce-메서드)
    - [화살표 함수와 'this'](#화살표-함수와-this) 
- [섹션 23: JavaScript의 최신 기능들](#섹션-23-javascript의-최신-기능들)
    - [기본 매개 변수](#기본-매개-변수)
    - [#함수 호출 시의 스프레드 구문](#함수-호출-시의-스프레드-구문)
    - [배열 리터럴 스프레드 구문](#배열-리터럴-스프레드-구문)
    - [객체 스프레드 구문](#객체-스프레드-구문)
    - [Rest 매개 변수](#rest-매개-변수)
    - [배열 분해](#배열-분해)
    - [객체 분해](#객체-분해)
    - [매개 변수 분해](#매개변수-분해)
- [섹션 24: DOM이란?](#섹션-24-dom이란)
    - [DOM 개요](#dom-개요)
    - [문서 오브젝트](#문서-오브젝트)
    - [getElementById](#getelementbyid)
    - [getElementsbyTagName & className](#getelementsbytagname--classname)
    - [querySelector & querySeletroAll](#queryselector--queryselectorall)
    - [innerHTML, textContent & innerText](#innerhtml-textcontent--innertext)
    - [속성 (Attribute)](#속성-attributes)
    - [스타일 변경하기](#스타일-변경하기)
    - [ClassList](#classlist)
    - [계층 이동](#계층-이동)
    - [Append & AppendChild](#append--appendchild)
    - [removeChild & remove](#removechild--remove)
- [섹션 25: 잃어버린 퍼즐 한 조각: DOM 이벤트](#섹션-25-잃어버린-퍼즐-한-조각-dom-이벤트)
    - [이벤트 개요](#이벤트-개요)
    - [인라인 이벤트](#인라인-이벤트)
    - [온클릭(OnClick) 속성](#온클릭onclick-속성)
    - [addEventListener](#addeventlistener)
    - [이벤트와 'this'라는 키워드](#이벤트와-this라는-키워드)
    - [키보드 이벤트와 이벤트 객체](#키보드-이벤트와-이벤트-객체)
    - [폼 이벤트 및 preventDefault](#폼-이벤트-및-preventdefault)
    - [입력과 변경 이벤트](#입력과-변경-이벤트)
    - [이벤트 버블링](#이벤트-버블링)
    - [이벤트 위임](#이벤트-위임)
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
- 함수를 정의하는 최신 구문
- `function` 키워드 없이도 함수를 입력할 수 있음 
```js
const sum = (x, y) => {
    return x + y;
}
```
- 인수가 1개일 때는 괄호가 없어도 됨
## 화살표 함수의 반환
- 함수의 바디에 표현식이 하나만 있을 경우 사용 가능
```js
const add = (a, b) => (
    a + b
)

const add = (a, b) => a +b
```
- 기존에 대괄호로 묶은 함수의 바디를 소괄호로 묶으면 `return`없이도 표현식의 값을 반환 함
## setTimeout과 setInterval
- 콜백 함수를 전달해야 하지만, 배열 메서드는 아님
### setTimeout
- 콜백 함수를, 설정한 값만큼 후에 실행 함
```js
setTimeout(() => {
    console.log("hi")
}, 3000)
// 3000ms 후에 'hi'를 출력
```
### setInterval
- 콜백 함수를 설정한 밀리 초마다 호출함
```js
setInterval(() => {
    console.log("hi")
}, 3000)
// 3000ms 마다 'hi'를 출력
```
- `clearInterval()`를 통해 멈출 수 있음
## Filter 메서드
- 요소로 구성된 배열에서 필터링을 하거나, 부분 집합을 모아 새 배열을 만드는데 사용
- 원본에 영향을 주지 않음
```js
const nums - [5, 4, 3, 2, 1];
const odds = nums.filter(n => {
    return n % 2 === 1;
})
// [5, 3, 1]
```
## Some과 every 메서드
### some
- 배열의 모든 요소가 콜백함수로 전달되어 한 요소라도 true을 반환하면, `some`함수도 true를 반환함
### every
- 배열의 모든 요소가 콜백함수로 전달되어 true을 반환하면, `every`함수도 true를 반환함
- 배열의 요소 중 하나라도 false라면 함수는 false를 반환
## 악명 높은 Reduce 메서드
- 배열을 점차 줄여가면서 하나의 값만 남기는 것
```js
 const evens = [2, 4, 6, 8];
 eves.reduce((sum, num) => sum + num)
 /* 2 + 4 = 6
 6 + 6 = 12
 12 + 8 = 20
 */
```
- 두 번째 인수를 추가해서 반환값(ex. sum)의 초기값을 설정할 수 있음
## 화살표 함수와 'this'
- 화살표 함수 안에 있는 `this`는 함수가 만든 범위를 가리킴
    - 객체 리터럴 안에 있는 함수에서 `this`를 사용하면 `window`객체를 가리킴
- 객체 리터럴 내의 함수를 정의할 때는 화살표 함수를 사용하면 안됨

# 섹션 23: JavaScript의 최신 기능들
## 기본 매개 변수
- 매개변수가 없을 때 디폴트 매개변수를 사용함
- 인수를 입력할 때 디폴트 값을 정의해줌
```js
funciton sum(a, b = 1) {
    return a + b;
}
```
## 함수 호출 시의 스프레드 구문
- 반복 가능한 객체를 확장해서 사용함
- 객체 앞에 `...`을 붙여서 사용
```js
Math.max(1, 3, 4, 6, 345)
// 345
const nums = [1, 3, 4, 6, 345]
Math.max(nums) // NaN
Math.max(...nums) // 345
```
## 배열 리터럴 스프레드 구문
- 기존의 배열을 스프레드 하여 새로운 배열을 만들 수 있음
```js
const nums1 = [1, 2, 3];
const nums2 = [4, 5, 6];

[...nums1, ...num2];
// [1, 2, 3, 4, 5, 6];
```
## 객체 스프레드 구문
- 객체의 특성을 복사하여 새로운 객체를 만듦
## Rest 매개 변수
- `Arguments`
    - 배열과 유사한 객체
    - 배열 메서드를 사용할 수 없음
- 배열 메서드를 사용하기 위해서 매개 변수에 `...`을 붙여 인수들을 배열로 나타냄
```js
function sumAll(...nums) {
    let total = 0;
    for (let n of nums) total += n;
    return total;
}

sumAll(1, 2, 3, 4, 5) //15
```
## 배열 분해
- 배열을 해체해서 별개의 변수 형태로 만들 수 있음
```js
const scores [199, 150, 130, 95, 23];

const [gold, silver] = scores;

gold; // 199
silver; // 150
```
## 객체 분해
- 객체의 프로퍼티나 매서드를 꺼내서 별개의 변수로 정의할 수 있음
- `프로퍼티명: 새로운이름`을 통해 변수명을 새로 정의할 수 있음
`프로퍼티명 = 디폴트값`을 통해 프로퍼티의 값이 없을 경우의 디폴트 값을 설정할 수 있음
```javascript
const runner = {
    first: "Eliud",
    last: "Kipchoge",
    age: 26,
}

const {first, last: "lastName",countr y= "IDK"} = runner;

first; // "Eliud"
lastName; // "Kipchoge"
country; // "IDK"
```
## 매개변수 분해

```js
const fullName = ({first, last}) => {
    return `$(first) $(last)`
}
fullName(runner); // "Eliud Kipchoge"
```
# 섹션 24: DOM이란?
## DOM 개요
- 문서 객체 모델
- 웹 페이지를 구성하는 JavaScript 객체들의 집합 
- JavaScript에서 웹 페이지의 콘텐츠로 접근하는 통로
- JavaScript를 통해 HTML과 CSS를 조작할 수 있음
## 문서 오브젝트
- 브라우저가 웹 페이지를 띄울 때 HTML과 CSS 정보를 받아들인 후 요소와 스타일을 기반을 JavaScript 객체를 생성함
- ex) HTML파일에 있는 `<body>`, `<h1>`, `<ul>`과 같은 요소들에 대한 고유한 JavaScript 객체가 생성됨
- 생성된 객체들은 각각의 객체들간의 부모자식 연결 관계를 가짐 
- Document 객체는 부모자식 관계의 최상위 객체
## getElementById
- String과 일치하는 Id를 가진 요소를 찾으면 해당 값을, 없으면 undefined를 반환함
- HTML, CSS요소를 직접 선택하는 것이 아닌, JavaScript를 통해 만들어진 DOM의 객체를 선택하는 것!!
## getElementsByTagName & className
- 한 번에 한 개 이상을 선택하기 때문에 Element's'
### getElementsByTagName
- 태그 이름을 전달하면 동일한 태그의 객체들을 원소로 가진 HTMLCollection을 반환 함
    - 반복 가능하지만 배열은 아님
### getElementsByClassName
- 전달된 클래스와 동일한 클래스의 객체들을 원소로 가진 HTMLCollection을 반환함
## querySelector & querySelectorAll
- 하나의 메서드를 사용해서 ID, 클래스, 태그, css 스타일, 속성등을 통해 객체들을 선택할 수 있음
- `querySelector`는 일치하는 첫 번째 요소를 반환
```js
// p태그를 선택
document.querySelector('p')
// Id가 banner를 선택
document.querySelector('#banner')
// Class가 square를 선택
document.querySelector('.square')
```
- `querySelectorAll`은 일치하는 첫 번째 요소가 아닌 모든 요소를 반환함
## innerHTML, textContent & innerText
### innerHTML
- 요소에 포함된 마크업의 전체 내용을 출력함
- 내용과 태그가 같이 나옴
### textContent
- `innerText`와 비슷한 역할을 함
- 요소 안에 있는 모든 요소가 나타남
### innerText
- 여는 태그와 닫는 태그 사이에 있는 내용을 텍스트로 보여줌
- ex) `<body>`를 선택하고 `innerText`를 했을 때는 `<body>`안에 있는 다른 태그의 내용은 보이지 않지만, `textContent`는 다 보임
## 속성 (Attributes)
- 요소의 특성에 직접 엑세스 하는 경우에는 JavaScript 객체를 가져 옴
### getAttribute()
- HTML 자체에서 속성을 직접 찾아옴
### setAttribute()
- 첫 번쨰 인수에 속성, 두 번째 인수에 새로운 값을 입력하여 속성 값을 수정함
## 스타일 변경하기
- style 객체에 속성들은 인라인 스타일들만 적용됨, 스타일시트의 속성들은 적용되지 않음 
## ClassList
-  JavsScript를 통해 직접 Style을 바꾸는 것은 인라인 스타일에만 적용되기 때문에 자주 사용하지 않음
- stylesheet에서 클래스마다 style을 지정하고, 객체에 클래스를 추가하는 방식으로 style을 변경할 수 있음
    - 적용할 클래스가 많아지면 이 방법 또한 번거로워 짐
- `classList`
    - 요소의 클래스를 제어, 검색 조작 함
    - `.add`를 통해 클래스를 추가
    - `.remove`를 통해 클래스를 제거
    - `.toggle`를 통해 적용된 클래스를 껐다 켰다 할 수 있음
## 계층 이동
- 주어진 요소에서 부모, 자식, 형제 요소에 접근
### parentElement
- 부모 요소에 접근함
### children
- 자식요소를 HTMLCollection으로 반환
### nextElementSibling
- 다음 형제 요소를 반환
### previousElementSibling
- 이전 형제 요소를 반환
## Append & AppendChild
### createElement
- 새로운 요소를 만듦
### appendChild
- 해당 요소에 자식 요소를 추가함
### append
- 한 개 이상의 요소를 추가할 수 있음
- 요소 뿐 만 아니라 텍스트, 이미지 또한 추가할 수 있음
### prepend
- 어떤 항목을 요소의 첫 번쨰 자녀로 삽입
### insertAdjacentElement
- 특정 위치에 항목을 요소로 삽입
## removeChild & remove
### removeChild
- 요소에서 자식을 제거
- 제거하려는 요소의 부모에 메서드를 호출해야 함
### remove
- 제거하려는 그 요소에 메서드를 호출
# 섹션 25: 잃어버린 퍼즐 한 조각: DOM 이벤트
## 이벤트 개요
- 이벤트 : 사용자들이 하는 행동에 반응하는 작업
- 클릭, 드래그, 스크롤, 키보드 입력 등 다양한 이벤트가 있음
## 인라인 이벤트
- html 태그내에 직접 이벤트를 작성
```html
<button onclick='alert("hi")' id='hi'></button>
```
## 온클릭(OnClick) 속성
- js 파일로 이벤트를 설정하는 방법
```js
const btn = document.querySelector('#hi')

btn.onclick = function() {
    console.log('hi')
}
```
- 이벤트에서 함수를 호출하여 실행하는 것이 아닌, 이벤트로 전달만 하는 것
```js
function scream() {
    console.log('ahahahah')
}

bth.onclick = scream
// not scream()
``` 
## addEventListener
-  이벤트를 추가할 때 가장 많이 쓰는 방법
- `addEventListener('이벤트', 콜백 함수)`
```js
const btn = document.querySelector('#hi')

btn.addEventListener('click', () => {
    alert('you clicked me')
})
```
- 다른 콜백 함수를 여러 줄에 써도 마지막으로 작성된 것 만 실행되지 않고 모두 실행됨
## 이벤트와 'this'라는 키워드
- `addEventListener`의 콜백 함수가 `this`를 가지고 있으면, `addEventListener`가 적용되는 요소에 콜백 함수가 실행됨
```js
function colorize() {
    this.style.backgorundColor = 'olive';
    this.style.color = 'white';
}

const btns = document.quersySelector('button')
for (let btn of btns) {
    btn.addEventListener('click', colorize)
}

const h1s = document.quersySelector('h1')
for (let h1 of h1s) {
    h1.addEventListener('click', colorize)
}
```
## 키보드 이벤트와 이벤트 객체
### 이벤트 객체
- `addEventListener`의 콜백 함수에 자동으로 전달됨
- 이벤트와 관련된 정보를 가지고 있음
### 키보드 이벤트
- `key`
    - 입력된 값
- `code`
    - 실제 키보드에서의 물리적인 위치
## 폼 이벤트 및 preventDefault
- `<form>`은 action 속성의 주소로 데이터를 전송하고, 브라우저에 보이는 페이지도 그 위치로 이동시킴
- 페이지를 이동시키는 것이 필요할 때도 있지만 필요하지 않을 수도 있음
- `Event.preventDefault`는 데이터 전송만 실행, 페이지 이동은 하지 않음
## 입력과 변경 이벤트
### change
- `input`에 무엇인가를 입력하고 입력창에서 나갔을 때 실행됨
### input
- `input`에 키를 입력할 때 마다 실행됨
- 화살표나 shift같이 실제 값에 영향을 주지 않을 때는 실행되지 않음
## 이벤트 버블링
- 하위 요소에서 발생한 이벤트가 상위 요소의 이벤트까지 영향을 미치는 것
- `e.stopPropagation`을 통해 막을 수 있음
## 이벤트 위임
- EventListener로 추가된 시점에 페이지에 없었던 요소를 다루는 방법
- 부모 요소에 EventListener를 추가
- `event.target`을 통해 정확히 이벤트를 실행시키는 요소를 정할 수 있음
# 섹션 27: 비동기식 JavaScript
## 콜 스택(Call Stack)
- Js 해석기가 사용하는 메커니즘
- 여러 함수를 호출하는 스크립트에서 해당 위치를 추적
- 