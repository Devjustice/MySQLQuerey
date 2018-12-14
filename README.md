# MySQLQuerey
마이시퀄 쿼리문 정리
데이터베이스 또는 테이블보기
SHOW DATABASES;
SHOW TABLES;

데이터베이스 생성하기
CREATE DATABASES 데이터베이스명;

테이블생성하기
CREATE TABLE 톄이블명 (칼럼명1, 칼럼명2 ,칼렴명3 ....칼럼명n);

데이터배이스 사용
USE 데이터베이스명;

데이터베이스 삭제하기
DROP DATABASE 데이터베이스명;

테이블 삭제하기
DROP TABLE 테이블명;

테이블에 세로운컬럼 추가하기
ALTER TABLE 테이블명 ADD 칼럼명 자료형;

테이블의 특정 컬럼을 변경하기
ALTER TABLE 테이블명 CHANGE 변경전명 변경후명 자료형;

테이블에 특정 컬럼을 삭제하기
ALTER TABLE 테이블명 DROP 칼럼명;

테이블에 데이터 추가하기
INSERT INTO 테이블명(칼럼1,칼럼2,..칼럼N)VALUES(데이터1,데이터2...데이터N);

테이블구조살펴보기
DESCRIBE 테이블명;

원하는 항목 표시하기 ->
SELECT*FROM 테이블이름;
SELECT 칼럼1,칼럼2,칼럼N FROM 테이블이름;

조건하에 항목표시하기
SELECT id,name,email FROM memo WHERE sex='M' AND math>'70';

순서대로 표시하기
//오름차순
SELECT name,phone FROM memo OREDR by 칼럼명 ASC;
//내림차순
SELECT name, phome FROM memo ORDER by 칼럼명 DESC;



원하는 갯수만큼 가저오기
//위에서 4개만 가져온다.
SELECT*FROM memo LIMIT 4;
//3번부터 4개만 가져온다.
SELECT*FROM memo LIMIT 2,4;


데이터 개수 알아내기

SELECT COUNT(*)FROM data;

특정조건에 해당되는 데이터 갯수 구하기.

SELECT COUNT(*)FROM data WHERE sex='F';

검색을 통해 데이터 가져오기

SELECT*FROM student WHERE name LIKE '사람%';

자료 업데이트하기
UPDATE 테이블명 SET 칼럼= 값...WHERE 조건문

자료 삭제하기
DELETE FROM 테이블명 WHERE 조건문;












