# The Web Developer 부트캠프 2023 - BE
# 목차
- [섹션 30: 터미널 완벽 정리](#섹션-30-터미널-완벽-정리)
    - [터미널 명령이란?](#터미널-명령이란)
    - [터미널 명령을 알아야 하는 이유](#터미널-명령을-알아야-하는-이유)
    - [기본 터미널: LS와 PWD](#기본-터미널-ls와-pwd)
    - [디렉터리 변경하기](#디렉토리-변경하기)
    - [상대 경로와 절대 경로](#상대-경로와-절대-경로)
    - [디렉터리 생성하기](#디렉토리-생성하기)
    - [맨(Man) 페이지와 플래그](#맨man-페이지와-플래그)
    - [터치 명령](#터치-명령)
    - [파일 및 폴더 제거하기](#파일-및-폴더-제거하기)
- [섹션 31: 우리의 첫 번째 도구: 노드 (Node)](#섹션-31-우리의-첫-번째-도구-노드-node)
    - [Node REPL](#node-repl)
    - [프로세스와 Argv](#프로세스와-argv)
    - [파일 시스템 모듈의 충돌 과정](#파일-시스템-모듈의-충돌-과정)
- [섹션 32: 모듈과 NPM](#섹션-32-모듈과-npm)
    - [Module.exports 사용하기](#moduleexports-사용하기)
    - [디렉터리의 필요성](#디렉터리의-필요성)
    - [NPM 개요](#npm-개요)
    - [패키지 설치하기](#패키지-설치하기)
    - [글로벌 패키지 추가하기](#글로벌-패키치-추가하기)
    - [Package.json의 중요성](#packagejson의-중요성)
    - [한 프로젝트에 대한 모든 종속 요소 설치하기](#한-프로젝트에-대한-모든-종속-요소-추가하기)
- [섹션 33: Express로 서버 제작하기](#섹션-33-express로-서버-제작하기)
    - [우리의 첫 번째 Express 앱](#우리의-첫-번쨰-express-앱)
    - [요청 및 응답 객체](#요청-및-응답-객체)
    - [Express 라우팅 기초](#express-라우팅-기초)
    - [Express 경로 매개 변수](#express-경로-매개-변수)
    - [쿼리 문자열 작업하기](#쿼리-문자열-작업하기)
    - [Nodemon을 사용한 자동 재시작](#nodemon을-사용한-자동-재시작)
- [섹션 34: 템플레이팅으로 동적 HTML 구성하기](#섹션-34-템플레이팅으로-동적-html-구성하기)
    - [템플레이팅이란?](#템플레이팅이란?)
    - [EJS용 Express 구성하기](#esj용-express-구성하기)
    - [뷰 디렉토리 설정하기](#뷰-디렉터리-설정하기)
    - [EJS 보간 구문](#ejs-보간-구문)
    - [템플릿에 데이터 전달하기](#템플릿에-데이터-전달하기)
    - [EJS의 조건문](#ejs의-조건문)
    - [EJS의 루프](#ejs의-조건문)
    - [Express의 정적 Assets 사용하기](#express의-정적-assets-사용하기)
    - [EJS와 파일 분할](#ejs와-파일-분할)
- [섹션 35: RESTful라우트 정의하기](#섹션-35-restful라우트-정의하기)
    - [Get 요청과 Post 요청](#get-요청과-post-요청)
    - [Express Post 경로 요청하기](#express-post-경로-정의하기)
    - [요청 구문 분석하기](#요청-구문-분석하기)
    - [RESTful 주석 개요](#restful-주석-개요)
    - [RESTful 주석 New](#restful-주석-new)
    - [Express 방향 수정](#express-방향-수정)
    - [RESTful 주석 Show](#restful-주석-show)
    - [UUID 패키지](#uuid-패키지)
    - [RESTful 주석 Update](#restful-주석-update)
    - [Express 메서드 재정의](#express-메서드-재정의)
    - [RESTful 주석 Delete](#restful-주석-delete)
- [섹션 36: 우리의 첫 번째 데이터베이스: MongoDB](#섹션-36-우리의-첫-번째-데이터베이스-mongodb)
    - [데이터베이스 개요](#데이터베이스-개요)
    - [SQL과 NoSQL 데이터베이스](#sql과-nosql-데이터베이스)
    - [Mongo를 배워야 하는 이유](#mongo를-배워야-하는-이유)
    - [Mongo Shell](#mongo-shell)
    - [BSON이란?](#bson이란)
    - [Mongo 데이터베이스에 삽입하기](#mongo-데이터베이스에-삽입하기)
    - [Mongo 데이터베이스에서 찾기](#mongo-데이터베이스에서-찾기)
    - [Mongo 데이터베이스 업데이트하기](#mongo-데이터베이스-업데이트하기)
    - [Mongo 데이터베이스에서 삭제](#mongo-데이터베이스에서-삭제)
    - [기타 Mongo 연산자](#기타-mongo-연산자)
- [섹션 37: Mongoose로 MongoDB에 접속하기](#섹션-37-mongoose로-mongodb에-접속하기)
    - [Mongoose란?](#mongoose란)
    - [Mongo에 Mongoose를 연결하기](#mongo에-mongoose를-연결하기)
    - [우리의 첫 번째 Mongoose 모델](#우리의-첫-번째-mongoose-모델)
    - [대량 삽입하기](#대량-삽입하기)
    - [Mongoose로 찾기](#mongoose로-찾기)
    - [Mongoose로 업데이트하기](#mongoose로-업데이트하기)
    - [Mongoose로 삭제하기](#mongoose로-삭제하기)
    - [Mongoose 스키마 유효성 겁사](#mongoose-스키마-유효성-검사)
    - [추가 스키마 제약조건](#추가-스키마-제약-조건)
    - [Mongoose 업데이트 유효성 검사하기](#mongoose-업데이트-유효성-검사하기)
    - [Mongoose 유효성 검사 오류](#mongoose-유효성-검사-오류)
    - [인스턴트 메서드](#인스턴스-메서드)
    - [정적 메서드 추가하기](#정적-메서드-추가하기)
    - [가상 Mongoose](#가상-mongoose)
    - [Mongoose를 미들웨어로 정의하기](#mongoose를-미들웨어로-정의하기)
# 섹션 30: 터미널 완벽 정리
## 터미널 명령이란?
- 터미널
    - 텍스트를 통해 내 기기와 상호작용 할 수 있는 텍스트 기반 프롬포트
## 터미널 명령을 알아야 하는 이유
1. 속도
- 터미널을 사용하여 GUI를 사용할 때 보다 더 빠르게 작업할 수 있음
2. 엑세스 
- 터미널을 사용하여 엑세스 권한을 가지고 OS나 접근금지 설정 등에 접근할 수 있음
3. 도구
- Node, Express, db와 같은 기술들이 대부분 터미널 기반임
## 기본 터미널: LS와 PWD
### LS
- 현재 있는 디렉터리의 콘텐츠를 나열함
### PWD
- Print Working Directory
- 현재 디렉터리를 알려줌
## 디렉터리 변경하기
### CD
- Change Directory
- 디렉터리를 앞, 뒤로 변경할 때 사용
- `cd ..` : 한 디렉터리 뒤로가기
## 상대 경로와 절대 경로
### 상대 경로
- 현재 위치에 따라 사용하는 경로
- 현재 위치를 기준으로 앞, 뒤로 움직일 수 있음
### 절대 경로
- 루트 디렉터리에서 `/`로 시작
- 어느 폴더에서라도 사용 할 수 있음
## 디렉터리 생성하기
### MKDIR
- Make Directory
- 디렉터리 이름을 입력해 빈 폴더를 생성함
- 공백을 통해 여러 폴더를 생성할 수 있음
## 맨(Man) 페이지와 플래그
### MAN
- manual
- `man 명령어`를 입력하면 명령어에 대한 정보 페이지를 출력함
### 플래그
- 명령어의 동작을 바꾸기 위해 입력함
- 명령어 뒤에 `-문자` 형식으로 입력
    - ex) ls -l, mkdir -v, ls -a
- 두 플래그를 한 번에 쓸 수도 있음
    - ex) ls -la
## 터치 명령
### Touch
- 파일을 생성함
- 공백을 통해 여러 파일을 생성할 수 있음
## 파일 및 폴더 제거하기
### Rm
- 파일을 영구 삭제함
- 공백을 통해 여러 파일을 삭제할 수 있음
### Rmdir
- 폴더를 영구 삭제함
- 빈 폴더에만 사용할 수 있음
- `rm -rf`를 사용하여 파일이 있는 폴더도 삭제할 수 있음
- 공백을 통해 여러 폴더를 삭제할 수 있음
# 섹션 31: 우리의 첫 번째 도구: 노드 (Node)
## Node REPL
- Node.js를 실행했을 때 터미널 상에서의 위치
- Dom APi, document, window 등과 같이 브라우저에서 기능하지만 Node에서 사용할 수 없는 기능도 있음
- Node의 전역 객체는 `global`
## 프로세스와 Argv
### Process
- 현재 실행하는 Node.js에 대한 정보와 그것의 실행을 통제하는 메서드를 가진 전역 객체
### Argv
- 배열을 반환
- Node를 실행할 수 있는 특성, 실행하고 있는 파일의 경로, 추가한 명령줄 인수로 구성됨
## 파일 시스템 모듈의 충돌 과정
### Fs
- File System
- 파일을 생성, 추가 등을 할 수 있는 모듈
- 모듈을 사용할 때에는 `require`를 사용하여 변수에 저장해야 함
    - `const fs = require('fs');`
# 섹션 32: 모듈과 NPM
## Module.exports 사용하기
- Js파일의 내용을 다른 Js 파일로 내보낼 때 사용
- `require`을 통해 파일을 불러올 때 가져오는 객체
```js
// math.js
module.exports.add = (x,y) => x + y;

// app.js
const math = require('./math');
math.add(2,3); 
```
## 디렉터리의 필요성
- 폴더 밖에서 폴더에 접근할 떄 `index.js`의 내용을 내보냄
    - `index.js`의 `module.exports`를 내보냄
## NPM 개요
- Node Pacakge Manager
- 많은 패키지로 된 라이브러리
    - 다른 사람들이 작성해 놓은 코드, 도구들을 설치하여 사용할 수 있음
- 명령줄 도구
    - 패키지를 손쉽게 설치 및 관리 할 수 있음
## 패키지 설치하기
- `npm install (패키지명)`
- `node_modules`폴더에 패키지의 코드와 패키지가 의존하는 다른 코드들이 설치됨
## 글로벌 패키치 추가하기
- 위의 패키치 설치 방법은 지역 설치 방법
    - 다른 디렉터리에서는 사용할 수 없음
- `npm install -g (패키지명)`를 사용하여 전역 설치 할 수 있음
    - 컴퓨터의 전역 `node_modules` 폴더에 설치됨  
## Package.json의 중요성
- 특정 프로젝트나 패키지, 앱에 대한 정보를 가지고 있는 파일
- `npm init`을 통해 package.json 파일을 만들 수 있음
- 패키지를 설치하면 `dependencies`에 자동으로 추가됨
## 한 프로젝트에 대한 모든 종속 요소 추가하기
- 다른 사람이 만든 코드를 다운 받을 경우, `node_modules`을 공유하는 경우는 잘 없음
- `npm install`을 실행하면 공유받은 파일의 `package.json`의 `dependencies`를 확인 후, 없는 패키지와 의존성들을 모두 설치함
# 섹션 33: Express로 서버 제작하기
## 우리의 첫 번쨰 Express 앱
```js
const express = require("express");
const app = express();

app.use(() => {
	console.log("i got a new request")
})

app.listen(3000, () => {
	console.log('hi hello');
})
```
- `listen()`
    - 앱이 요청을 받거나 인수로 받은 포트로 요청을 받으면 콜백함수를 실행함
- `use()`
    - 요청이 들어오면 콜백이 실행됨
    - 요청이 어디서 오든 상관 없음
## 요청 및 응답 객체
- req, res
    - express에서 만드는 객체들
    - HTTP 요청은 Js객체가 아니기 때문에 express가 데이터를 파싱해서 전달할 객체로 변환 함
- res.send()
    - HTTP 응답을 생성하고 보냄
    - 어떤 종류의 요청이라도 반응함
## Express 라우팅 기초
### 라우팅
- 요청과 요청된 경로를 가져와서 응답을 갖는 어떠한 코드에 맞추는 것
    - ex) /help => "고객센터", /home => "홈페이지"
### `app.get(요청 경로, 콜백)`
- 요청 경로에 맞는 HTTP 요청이 들어왔을 때 콜백함수를 실행함
## Express 경로 매개 변수
- 라우트를 패턴화 할 때 사용
    - ex) reddit : r/chickens, r/soccer ...
- 경로 문자열에 `:`을 사용하여 변수로 만듦
```js
app.get('/r/:subreddit', ())
```
- `req.params`를 통해 변수에 접근할 수 있음
```js
// r/cats 요청을 했을 때
{ subbreddit : 'cats'}
```
## 쿼리 문자열 작업하기
- `req.query`를 통해 접근할 수 있음
## Nodemon을 사용한 자동 재시작
- nodemon 라이브러리를 사용하여 js파일에 변경사항이 있을 때 서버를 자동으로 재시작 하게 만들 수 있음
# 섹션 34: 템플레이팅으로 동적 HTML 구성하기
## 템플레이팅이란?
- 정보와 로직을 넣어서 동적으로 HTML을 사용하는 것
## ESJ용 Express 구성하기
- `app.set('view engine', 'ejs')`
    - 앱에 EJS를 사용한다고 알림
- npma을 통해 EJS를 설치
- Express views 디렉터리에 템플릿이 있다고 디폴트로 설정함
    - view파일 안에 ejs파일을 만들어 템플릿 설정
- `res.render`
    - view를 렌더링하고 렌더링 된 HTMl 문자열을 클라이언트에 보냄
## 뷰 디렉터리 설정하기
- view 디렉터리의 바로 위의 파일이 아닌 곳에서 서버를 실행하면 오류가 발생
```JS
const path = require('path');

app.set('views', path.join(__dirname, '/views'))

```
- js파일이 있는 현재 디렉터리를 가져와서 거기에 도달하기 위한 전체 디렉터리에 /view를 붙여줌
## EJS 보간 구문
### <%= %>
- 태그 안에 내용들은 js로 취급함
## 템플릿에 데이터 전달하기
- `res.render`에서 두 번째 인수로 키-값 쌍 객체를 보낼 수 있음
- js파일에서 정의한 값을 ejs파일의 키로 보낼 수 있음
```js
// index.js
app.get('/rand', (req,res) => {
    const num = Math.floor(Math.random() * 10) + 1;
    res.render('random', {num : num})
})
```
```html
// random.ejs
<h1>Random number is <%= num %></h1>
```
## EJS의 조건문
### <% %>
- 태그 안에 내용들을 js로 임베드 하되 템플릿에 추가하지 않음
```html
<h1>
    Your random number is: <%= num %>
</h1>
<% if(num % 2 === 0) { %>
<h2>
    Tha is an even number!
</h2>
<% } else { %>
<h2>
    Tha is an odd number!
</h2>
<% } %>
``` 
- 기존 js에서 if, else 구문을 `<% %>`로 감싸면 됨
## EJS의 루프
```html
<ul>
    <% for(let cat of cats) { %>
    <li><%= cat %></li>
    <% } %>
</ul>
```
- 조건문과 마찬가지로 js 내용을 `<% %>`로 묶음
## Express의 정적 Assets 사용하기
- css, js, img 등의 파일을 클라이언트 측에 전달할 때 사용
- `app.use(express.static('public'))`
- 파일들이 들어있는 public 디렉터리를 전달
- `path.join(__dirname, 'public')`
    - 다른 디렉터리에서 서버를 실행할 때의 오류를 방지
## EJS와 파일 분할
- `<%- include(디렉터리) %>`
- 이스케이프가 되지 않은 값을 템플릿에 출력
    - 이스케이프 : 콘텐츠를 문자열로 취급할 때 
- ex) html의 `<head>`를 ejs파일로 따로 만든 후 각각의 라우팅 `<head>`를 위의 코드로 대체할 수 있음
# 섹션 35: RESTful라우트 정의하기
## Get 요청과 Post 요청
### get
- 정보를 가져올 때 사용
- 요청을 보낼 때 같이 따라오는 데이터는 쿼리 문자열에 담김
### post
- 정보를 올리거나 보낼 때 사용
- 같이 따라오는 데이터는 쿼리 문자열이 아닌 요청의 body에 포함됨
## Express Post 경로 정의하기
- `app.post`를 통해 POST 요청을 받았을 때 행동을 정의할 수 있음
## 요청 구문 분석하기
- `req.body`
    - request body에 제출된 데이터의 키-값 쌍을 포함
    - 기본값 : undefined
    - body 분석 미들웨어 사용 시 추가됨
        - ex) express.json(), express.urlencoded()...
## REST 개요
- Representational State Transfer
- 클라이언트와 서버가 어떻게 서로 소통해야 하는가에 대한 가이드라인, 개념, 원리
- RESTful : REST 규칙에 따르는 시스템
- 리소스 : 하나의 엔티티
    - ex) 트윗, 사용자, 이미지...
- 인터페이스 일관성 : 다른 HTTP 동사를 일관된 URL 패턴과 매치햐여 구성하는 것
## RESTful 주석 개요
- 댓글을 CRUD하는 api를 만듦
- HTTP 동사를 기본 URL과 필요시 ID도 매치
```
GET /comments - 모든 댓글 출력
POST /comments - 새 댓글 작성
GET /comments/:id - 특정 댓글 출력
PATCH /comments/:id - 댓글 수정
DELETE /comments/:id - 댓글 삭제
``` 
## RESTful 주석 New
```js
app.post('/comments', (req, res) => {
	const { username, comment } = req.body;
	comments.push({ username, comment, id: uuid() })
	res.redirect('/comments');
})
```
## Express 방향 수정
- `res.redirect()`
- 지정한 url로 리다이렉트 함
- 302(defalut) 상태코드를 받으면 초기 응답에서 전송된 위치를 기반으로 이어서 진행함
- HTTP 응답 header에 지정한 url를 포함하여 이후 그 url로 GET 요청을 함
## RESTful 주석 Show
```js
app.get('/comments/:id', (req, res) => {
	const { id } = req.params;
	const comment = comments.find( c => c.id === id)
	res.render('comments/show', { comment })
})
```
## UUID 패키지
- 고유 식별자를 생성해주는 패키지
## RESTful 주석 Update
```js
app.patch('/comments/:id', (req, res) => {
	const { id } = req.params;
	const newCommentText = req.body.comment;
	const foundComment = comments.find( c => c.id === id);
	foundComment.comment = newCommentText;
	res.redirect('/comments');
})
```
- url에 입력된 id를 req.params을 통해 가져옴
- req.body.comment에 담긴 페이로드, 즉 수정할 내용을 가져옴
- 기존 DB에서 url에 입력된 id와 동일한 id를 가진 댓글을 찾음
- 댓글의 내용을 페이로드의 내용으로 정의
- index페이지로 redirect
## Express 메서드 재정의
- html의 form에서는 delete, patch, put 등의 메서드를 사용할 수 없음
- mehtod-override
    - 클라이언트가 해당 작업을 지원하지 않는 환경에서 HTTP 동사를 사용할 수 있게 해주는 패키지
```js
// js
const methodOverride = require('method-override');

app.use(methodOverride('_method'))
```
```html
// ejs
<form method='POST' action='/comments/<%=comment.id%>?_method=PATCH'></form>
```
## RESTful 주석 Delete
```html
// ejs
<form method="POST" action="/comments/<%= comment.id %>?_method=DELETE">

```
# 섹션 36: 우리의 첫 번째 데이터베이스: MongoDB
## 데이터베이스 개요
- DB는 많은 양의 데이터를 효율적으로 저장하고 압축하여 관리하기 쉽고, 접속하기 쉽게 만들어 줌
- DB가 제공하는 다양한 도구들을 사용하여 데이터를 쉽게 삽입, 조회, 갱신, 삭제, 정렬 등을 할 수 있음
- 데이터의 액세스를 관리하는 보안 기능을 제공
## SQL과 NoSQL 데이터베이스
### SQL
- Structured Query Language
- 기본적인 구문을 공유하는 관계형 데이터베이스
- ex) MySQL, Postgres, Oracle ...
- 테이블을 만들고 개별 요소를 정의
- 다른 테이블에 있는 그 요소들을 연결하여 서로 참조하도록 함
### NoSQL
- SQL의 구조화된 언어를 쓰지 않고, 많은 요소를 포괄하는 방식
- ex) MongoDB, Redis ...
## Mongo를 배워야 하는 이유
- Monogo가 Node, Express를 사용할때 많이 사용됨
- 배우기 쉬움
- Js와 쓰기 쉬움 
## Mongo Shell
- Node의 RELP처럼 터미널에서 사용하는 Mongo
- `use db명`
    - 빈 db를 만듦  
## BSON이란?
- 이진법 JSON
- JSON을 압축하여 공간을 더 적게 활용함
## Mongo 데이터베이스에 삽입하기
### db.collection.insertOne()
- 객체 하나를 db에 삽입함
```mongo
db.dogs.inserOne({name: "Charlie", age: 3, breed: "corgi", catFriendly: true})
```
- collection을 확인하면 추가하지 않은 "_id"가 추가되어 있음
    - objectId
    -  Mongo에 의해 자동 생성
    - 기본 키
### db.collection.insert()
- 하나의 문서나, 객체 혹은 다수의 문서를 db에 전달함
```mongo
db.dogs.insert([{name: "Wyatt", breed: "Golden", age: 14, catFriendly: fa
lse},{name: "Tonya", breed: "Chihuahua", age: 17, catFriendly: true}])
```
## Mongo 데이터베이스에서 찾기
### db.collection.find()
- 컬렉션의 모든 요소 또는 문서를 보여줌
- 인수에 객체를 넣어 객체에 해당하는 요소만 찾을 수 있음
- 커서(결과의 참조)를 반환함
```mongo
db.dogs.find({breed: 'Corgi'})
```
## Mongo 데이터베이스 업데이트하기
### db.collection.updateOne/updageMany
- 매치되는 첫/모든 항목을 업데이트
- 두 가지 인수 필요
    - 찾는 문서와 매치되는 특징
    - 변경 내용
- 변경 내용에는 특수 연산자를 활용해야 함
- $set : 필드의 값을 새로운 값으로 대체하거나 추가할 때 사용
```mongo
db.dogs.find({breed: 'Corgi'}, {$set: {age: 5}})
```
- 기존에 없던 내용을 입력하면 새로 추가됨
### db.collection.replaceOne
- `_id`는 유지한 채로, 모든 내용을 바꿀 때 사용
## Mongo 데이터베이스에서 삭제
### db.collection.deleteOne/Many
- 기준에 따라 항목을 하나/모두 삭제함
```mongo
db.dogs.deleteOne({breed: 'Corgi'})
``` 
- `deleteMany`에 인수로 `{}`를 넣으면 모든 항목을 삭제함
### 기타 Mongo 연산자
- 객체의 값으로 검색을 할 때는 키를 따옴표로 묶어야 함
```mongo
db.dogs.findOne({'personality.childFriendly': true})
```
### $gt/gte/lte/lt
- 비교 연산자(초과/이상/이하/미만)
- `db.dogs.find({age: {$gt: 8}})`
### $in/nin
- 배열 안에 어떤 값이 포함되어 있는/없는 문서를 선택
- `db.dogs.find({breed: {$in: ['Corgi', 'Mutt']}})`
# 섹션 37: Mongoose로 MongoDB에 접속하기
## Mongoose란?
- ODM
    - Object Data/Document Mapper(객체 데이터/문서 매퍼)
- Mongo와 Node를 연결해줌
- 데이터나 문서를 Js 객체로 매핑
- 기존 Mongo를 개선하여 Js에서 유용한 기능을 추가해줌
## Mongo에 Mongoose를 연결하기
```js
const mongoose = require('mongoose');
mongoose.connect('mongodb://127.0.0.1:27017/test')
	.then(() => {
		console.log('connection open')
	})
	.catch(err => {
		console.log('error')
		console.log(err)
	})
```
## 우리의 첫 번째 Mongoose 모델
```js
const movieSchema = new mongoose.Schema({
	title: String,
	year: Number,
	score: Number,
	rating: String
});

const Movie = mongoose.model('Movie', movieSchema);

const amadeus = new Movie({ title: 'Amadeus', year: 1986, score: 9.2, rating: 'R'})
```
- 모델
    - Mongoose의 도움으로 생성되는 Js 클래스
    - MongoDB의 정보를 나타냄
- 스키마
    - Mongo의 각기 다른 키 집합을 Js의 다른 타입으로 구조를 짜는 것
- mongoose.model('모델이름', 스키마)
    - 모델이름
        - 단수형, 첫 문자는 대문자
        - mongoose가 이름을 바탕으로 자동으로 복수형 집합을 생성함
- node에서 `.load 파일명`을 통해 파일을 실행, `객체명.save()`로 Mongo에 저장할 수 있음
## 대량 삽입하기
### insertMany 
- 실제로 쓰는 일은 잘 없음
- 단일 객체를 저장할 때 `save()`를 해야 했던 것과 달리, 유효성 검사를 통과후 바로 Mongo에 저장됨
```js
Movie.insertMany([
	{ title: 'Amelie', year: 2001, score: 8.3, rating: 'R'},
	{ title: 'Alien', year: 1979, score: 8.1, rating: 'R'},
	{ title: 'The Iron Giant', year: 1999, score: 7.5, rating: 'PG'},
	{ title: 'Stand By Me', year: 1986, score: 8.6, rating:'R'},
	{ title: 'Moonrise Kingdom', year: 2012, score: 7.3, rating: 'PG-13'}
])
	.then(data => {
		console.log('It Worked');
		console.log(data);
	})
```
## Mongoose로 찾기
### find()
- 키-값 쌍을 통해 데이터를 하나 혹은 여러 개 찾음
- `.then`을 사용하지만 Promise는 아님
```mongo
Movie.find({year: {gte: 2015}}).then(data => console.log(data))
```
- find는 쿼리 객체를 반환하기 떄문에 원하는 데이터를 보기 위해서는 `.then`을 사용해야 함
- data는 배열로 반환 됨
### findOne()
- 키-값 쌍을 통해 데이터를 하나 만 반환
```mongo
Movie.findOne({year: {gte: 2015}}).then(data => console.log(data))
```
### findById()
- `_id`를 통해 데이터를 검색
- 보통 api를 만들 때 id를 사용하여 만드는 경우가 많기 때문에 유용하게 사용됨
## Mongoose로 업데이트하기
### updateOne/Many()
- 쿼리에 매치되는 첫 번째 모든 항목을 갱신함
- updateOne({검색 기준}, {변경 내용})
- 갱신된 정보를 반환하지 않고, 수정 여부만을 알리는 객체를 반환함
    - ex) `{n: 2, nModified: 2, ok: 1}`
### findById/OneAndUpdate()
- 쿼리에 매치되는 항목을 갱신함
- 갱신된 내용을 보기 위해선 `{new : true}`를 인수로 보내야 함
```mongo
> Movie.findOneAndUpdate({title: 'The Iron Giant'}, {score: 10.0}, {new: true}).then(m => console.log(m))
```
## Mongoose로 삭제하기
### deleteOne/Many
- 쿼리에 매치되는 한/모든 항목을 삭제함
```mongoose
Movie.deleteMany({year: {$gte: 1999}}).then(msg => console.log(msg))
``` 
- 갱신된 정보를 반환하지 않고, 수정 여부만을 알리는 객체를 반환함
### findById/OneAndDelete()
- 쿼리에 매치되는 항목을 삭제함
- 삭제된 항목을 반환 함
## Mongoose 스키마 유효성 검사
```js
const productSchema = new mongoose.Schema({
	name: {
		type: String,
		required: true
	},
	price: {
		type: Number,
	}
});
```
- 스키마를 정의할 때 중괄호를 통해 더 구체적으로 값을 정할 수 있음
- `require`특성을 지닌 키는 문서를 만들 때 반드시 정의되어야 함
## 추가 스키마 제약 조건
- default
    - 문서 정의 때 값이 입력되지 않으면 default값을 사용함
- min/max
    - 최소/최대 값
- 키-값 쌍이 중첩되고 각각에 타입을 정할 수도 있음
## Mongoose 업데이트 유효성 검사하기
- 유효성 검사는 만들 때만 적용, 업데이트되고 나서는 Mongoose에게 계속 유효성 검사를 진행하라고 말해야 함
- `{runValidators: true}`
## Mongoose 유효성 검사 오류
- 내장 유효성 검사기에서 사용
- 값에 배열을 추가
    - 첫 번째 인수는 값, 두 번쨰 인수는 에러 메세지
```js
min: [6, 'Too few eggs']
```
## 인스턴스 메서드
- Mongoose가 제공하는 기능 외에 추가로 모델에 기능을 정의하거나 추가하는 방법
- `스키마.methods.메서드`
- 화살표 함수가 아닌 기존 함수 표현식을 사용해야 함
## 정적 메서드 추가하기
- 모델 자체에 적용하는 메서드
- `스키마.statics.메서드`
## 가상 Mongoose
- 실제 db 자체에는 존재하지 않는 스키마에 특성을 추가할 수 있게 함
- `스키마.virtual(특성명).get(콜백)`
## Mongoose를 미들웨어 정의하기
- 특정 작업 실행 전후에 코드를 실행할 수 있음
- `.pre`, `.post`
    - 코드 실행 전/후에 콜백을 실행
# 섹션 38: 하나로 묶기: Express와 Mongoose
## 프로덕트 인덱스
```js
app.get('/products', async (req, res) => {
	const products = await Product.find({});
	res.render('products/index', { products })
})
```
- `Product.find()`는 모든 상품을 다 찾는데, 이것을 하는데 시간이 걸림
- `async, await`를 통해 비동기로 만들어 찾는 것이 끝날 때 까지 다른 동작을 못하게 만듦
## 프로덕트 디테일
```js
app.get('/products/:id', async (req, res) => {
	const { id } = req.params;
	const product = await Product.findById(id);
	res.render('products/show', { product })
})
```
- `Product.findById()`를 통해 mongoose id를 통해 상품을 찾음
## 프로덕트 만들기