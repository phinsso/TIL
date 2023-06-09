## Database
- 데이터 저장소
- DBMS: 사용자가 DB를 사용하기 쉽게 관리해주는 프로그램
---
#### 접속 방법: **mysql -u아이디 -p비밀번호 사용할DB**
- 처음(아무런 내용도 없을 때)는 root로 접속
---
### 1. DB 생성
- **create database 생성할데이터베이스이름;**
- create database testdb;
### 2. 계정 생성 (비밀번호까지 설정)
- **create user 'test'@localhost identified by '1111';**
### 3. 계정과 DB 연동, 권한 부여
- **grant all privileges on testdb.* to test@'localhost' with grant option;**
### 4. 현재 접속 중인 DB 나가기
- exit
### 5. 새로 생성한 DB에 접속
- mysql -u아이디 -p비밀번호 새로생성한DB이름;
### 6. 테이블 만들기
- **create table 생성할테이블이름 (
	컬럼이름 자료형 조건;
                  )**

- 위에서 조건은 생략해도 됨.
