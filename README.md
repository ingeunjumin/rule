## 팀 인근주민 규칙 :running:


### daily 규칙
1. 매일 5~10분 커피타임(이슈 사항&오늘 todo 정리하는 타임!)
2. jira 업데이트 부터 하고 할일 하기

### team 규칙
1. 오전은 업무에 집중, 질문은 되도록 오후에 하기.
2. 식사시간은 프리하게. (먹는시간은 건들지 말자!)
3. sub-task은 3일을 넘기지 않는다. ex)  spring<-> mysql 연결 3일은... 너무하지 않소!
4. commit 내용은 상세하게. 
5. 모든 고민은 팀끼리. (급발진 ㄴㄴ)
6. 시간안에 못한 일은 명확하고 간단하게 PM에게 보고.

### dev 규칙
1. 모든 메소드와 변수 표기는 *카멜문법을 사용.  ex) userName
2. 메소드 이름은 *동사로 표현, 변수 이름은 *명사로 표현.
3. boolean형 변수와 return타입이 boolean형 메소드는 *is,*has 를 꼭 붙인다.
4. *축약어를 사용하지 말자. ex)유저 번호 변수 이름 :  userP(x) -> userPhoneNumber (o)
5. 상수 변수는 *대문자로 표기. ex) final int SECONDS_IN_A_DAY = 86400
6. 메소드 인수(argument,파라미터)는 *3개를 넘지 않는다. 넘을 경우 객체(class)를 이용하여 전달.
7. update, delete, insert 메소드에 @Transactional을 사용.
8. commet(주석)는 간단하게 메소드 만든사람 이름 꼭 쓰기.

### api 규칙
1. 슬래시(/) 구분자는 계층 관계를 나타내는 데 사용.
	ex) http://restapi.example.com/animals/mammals/whales
	
2. URL 마지막 문자로 슬래시(/)를 포함하지 않는다.
	ex) http://restapi.example.com/houses/apartments/ (X)
	    http://restapi.example.com/houses/apartments (0)
	    
3. 밑줄(_)은 URL에 사용하지 않는다. 대신 하이픈(-)을 사용하여 URL 가독성을 높이자!
	ex) http://restapi.example.com/users/game_list (X)
	ex) http://restapi.example.com/users/game-list (0)
	
4. URL 경로에는 소문자가 적합.	

5. 행위(method)는 URL에 포함하지 않는다.
	ex) http://restapi.example.com/users/update/info (X)
	ex) http://restapi.example.com/users/info (0)
	
6. 동사보다는 명사를 사용.  

7. 단수(Singular) 보다는 복수(Plural)형 명사를 사용.
	ex) http://restapi.example.com/sports/soccer/players/13