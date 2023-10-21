# The Web Developer 부트캠프 2023 - Mongo,Mongoose
# 목차
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
