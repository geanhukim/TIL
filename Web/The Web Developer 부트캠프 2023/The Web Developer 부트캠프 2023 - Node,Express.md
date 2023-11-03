# The Web Developer 부트캠프 2023 - Node,Express
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
- [섹션 40: 미들웨어: Express의 키(key)](#섹션-40-미들웨어-express의-키key)
    - [Express 미들웨어 개요](#express-미들웨어-개요)
    - [모건-로거(Morgan-Logger) 미들웨어 사용하기](#모건-로거morgan-logger-미들웨어-사용하기)
    - [미들웨어 정의하기](#미들웨어-정의하기)
    - [404 경로 설정](#404-경로-설정)
- [섹션 42: Express 앱의 오류 처리하기](#섹션-42-express-앱의-오류-처리하기)
    - [Express의 태생적 오류 처리기](#express의-태생적-오류-처리기)
    - [사용자 지정 오류 처리기 정의하기](#사용자-지정-오류-처리기-정의하기)
    - [사용자 지정 오류 클래스](#사용자-지정-오류-클래스)
    - [비동기 오류 처리하기](#비동기-오류-처리하기)
    - [비동기 오류 처리 더 알아보기](#비동기-오류-처리-더-알아보기)
    - [비동기 유틸리티 정의하기](#비동기-유틸리티-정의하기)
    - [Mongoose 오류 구분하기](#mongoose-오류-구분하기)
- [섹션 47: Express의 라우터와 쿠키]
    - [Express 라우터 개요]
    - [Express 라우터와 미들웨어]
    - [쿠키 개요]
    - [쿠키 보내기]
    - [쿠키 파서 미들웨어]
    - [쿠키 서명하기]
- [섹션 48: Express의 세션과 플래시]
    - [세션 개요]
    - [Express 세션]
    - [Express 세션 더 알아보기]
    - [플래시 개요]

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
# 섹션 40: 미들웨어: Express의 키(key)
## Express 미들웨어 개요
- 요청-응답 생명주기 내에서 실행되는 함수
- Express가 요청을받고 코드를 처리 후, 응답을 내보낼 때 까지 실행됨
- 미들웨어를 통해 요청-응답 생명주기를 종료하거나 미들웨어를 연쇄하여 실행할 수 있음
## 모건-로거(Morgan-Logger) 미들웨어 사용하기
### 모건(Morgan)
- http 요청을 터미널에 로그로 남겨주는 패키지
## 미들웨어 정의하기
- ex) `app.get('', (req, res, next))`
- 미들웨어 안에서 `next`를 호출하면 알맞은 미들웨어나 라우팅 핸들러가 실행됨
- `next()`를 return하면 next 밑에 있는 코드는 실행되지 않음
## 404 경로 설정
- `app.use`는 모든 요청에 대해 함수를 전달할 뿐만 아니라, 라우트 핸들러와 같이 특정 경로에 대해 함수를 전달할 수 있음
```js
app.use('/dogs', (req, res, next) => {
    console.log('i like dog');
    next();
})
```
- `/dogs`에 대해 어떠한 요청이 오더라도(GET, POST...) 실행됨

- 앱의 가장 마지막에 `app.use`를 활용하여 경로가 지정되지 않은 요청에 대한 404 상태 코드에 대한 응답을 보낼 수 있음
    - 해당하는 경로가 있을 경우에는 미들웨어보다 라우트 핸들러가 위에 있기 때문에 미들웨어가 실행되지 않음
# 섹션 42: Express 앱의 오류 처리하기
## Express의 태생적 오류 처리기
- Express는 빌트인 에러 핸들러가 앱에서 발생한 모든 에러를 처리함
## 사용자 지정 오류 처리기 정의하기
- 다른 미들웨어 처럼 오류 처리 미들웨어 함수를 만들 수 있음
- 4개의 인수를 필요로 함 (err, req, res, next)
- `app.use()`뒤 가장 마지막에 정의해야 함
- 오류가 나기만 하면 오류 처리 미들웨어가 실행됨
- next 오류 처리 미들웨어를 불러올 때는 `next(err)`를 통해 넘겨야 함
## 사용자 지정 오류 클래스
- 웹 앱에서는 오류에 대한 응답으로 상태코드와 메시지를 전달하는게 일반적
- 모든 오류마다 `res.status()`와 메시지를 각각 설정해 주는 것은 비효율적
    - 각기 다른 상황에서 발생하는 오류들을 모두 처리하기에는 번거로움
- 커스텀 오류를 발생하여 재사용에 용이하게 함
```JS
// AppError.js
class AppError extends Error {
	constructor(message, status) {
		super();
		this.message = message;
		this.status = status;
	}
}
module.exports = AppError;

// index.js 미들웨어
throw new AppError('Password required', 401)
```
- 빌트인 오류를 확장해서 사용
- 디폴트 오류 핸들러는 `err.status`를 찾아서 상태코드를 전달해줌
- Js 디폴트 Error 클래스에는 status가 없기 때문에 커스텀 오류를 만들 때 직접 입력 해 줘야 함

```js
app.use((err, req, res, next) => {
	const {status=500, message='Something Went Wrong'} = err;
	res.status(status).send(message)
})
```
- 오류 객체에 상태 코드가 없는 오류를 대비해 default 값을 정의해야 함
## 비동기 오류 처리하기
- 라우트 핸들러와 미들웨어에 의해 발동된 비동기 함수에서 반환된 오류는 `next()`로 전달해야 함
- `next()`로 오류 핸들러로 전달한 후 `next()` 뒤에 있는 코드가 실행 되어 다른 오류(ex. 컴파일 오류) 가 발생할 수 있음
    - `next()`를 `return`하여 뒤에 있는 코드가 실행되지 않게 만듦
## 비동기 오류 처리 더 알아보기
- AppError와 같은 커스텀 에러가 아닌 Mongoose에서 오는 오류나 우연이 생긴 오류 등 `next()`로 전달할 오류가 없는 경우도 있음
- try..catch 문을 활용함
```js
try{
    ...
}
catch(e) {
    next(e)
}
```
## 비동기 유틸리티 정의하기
- 비동기 함수를 인수로 하는 새로운 함수를 정의
```js
function wrapAsync(fn) {
    return function (req, res, next) {
        fn(req, res, next).catch(e => next(e))
    }
}
```
## Mongoose 오류 구분하기
- Mongoose가 발생시키는 에러는 `name` 특성을 가지고 있음
- 기존의 에러 핸들러와 다른 핸들러를 만들고, err.name이 특정 Mongoose 에러 메세지와 같을 때 실행될 함수를 만들어 따로 처리할 수 있음
# 섹션 47: Express의 라우터와 쿠키
## Express 라우터와 개요
- 이전에는 js파일 하나에 모든 라우트를 작성함
- express의 Router기능을 활용해 동일한 리소스를 공유하는 라우트를 한 파일에 넣어 더 효율적으로 관리 할 수 있음
```js
// shelter.js
const router = express.Router();

router.get('/', (req, rex) ...)
router.get('/:id', ...)
rotuer.post('/',...)
router.get('/:id/edit',...)

// index.js
app.use('/shelters', shelterRoutes);
```
- `router`객체를 활용하여 각 라우트에 해당 리소스를 직접 정의해 주지 않아도 적용이 가능함
## Express 라우터와 미들웨어
- 특정 라우트에만 미들웨어를 적용하고 싶은 경우가 있음
- 라우트 파일에서, 미들웨어를 정의할 때 사용하던 `app.use`를 `router.use`로 변경
- 해당 라우트가 아닌 다른 라우트에서는 미들웨어가 작동하지 않게 됨
## 쿠키 개요
- 사용자의 브라우저에 저장되는 작은 조각들
- HTTP는 모든 요청이 개별적 -> 이전의 요청을 기억하지 못함
- 쿠키를 사용해 브라우저의 일부 정보를 저장하고 이후 그 데이터를 서버에 보낼 때 사용할 수 있음
    - ex) 장바구니, 다크모드
## 쿠키 보내기
- `res.cookie('쿠키명', '쿠키값')`을 통해 브라우저에 쿠키를 전달할 수 있음
## 쿠키 파서 미들웨어
- cookie-parser 패키지를 통해 모든 요청에 `request.cookies`라는 특성이 포함됨
- `app.use(cookieParser())`
## 쿠키 서명하기
- 서명 : 정보가 변하지 않았음을 확인하는 방식
- 쿠키 파서가 비밀코드로 쿠키에 서명
- 서명된 쿠키를 클라이언트 측에서 다른 쿠키들과 마찬가지로 돌려줌
- 서버 측에서는 서명된 쿠키를 살펴보아 누군가 쿠키를 건들이지 않았는지 확인함
- `res.cookie()`에 `{signed: true}`를 인수로 추가함
- 서명된 쿠키는 `req.cookies`에서 확인할 수 없음
    - `req.signedCookies`에서 확인 가능