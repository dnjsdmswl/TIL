# ERD 표기법

Entity Relationship Diagram (존재하고 있는 것들의 관계를 나타낸 도표)

![img.gif](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img.gif)

![IE 표기법과 Barker 표기법](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn.png)

IE 표기법과 Barker 표기법

## ERD 엔티티 표기법

![엔티티/정의 가능한 사물 또는 개념](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%201.png)

엔티티/정의 가능한 사물 또는 개념

![엔티티 속성(Attribute)](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%202.png)

엔티티 속성(Attribute)

![엔티티 도메인(Domain) / 속성 타입 그리기 or 생략](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%203.png)

엔티티 도메인(Domain) / 속성 타입 그리기 or 생략

![img1.daumcdn.png](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%204.png)

유형 엔티티 : 물리적인 형태 ex)고객 정보

무형 엔티티 : 물리적인 형태 X, 개념적으로만 존재 ex)구매 이력

![주 식별자(Primary Key) - PK](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%205.png)

주 식별자(Primary Key) - PK

중복 X, NULL값 X → 유일한 값에 지정하는 식별

◆ 다이아몬드나  **🔑**열쇠로 표현

![NOT NULL](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%206.png)

NOT NULL

해당 속성에

NULL 허용 → 비워두기

NULL 비허용 → N or NN 적기

![외래 식별자(Foreign Key) - FK](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%207.png)

외래 식별자(Foreign Key) - FK

외래 식별자도 key의 일종 → **🔑**열쇠 아이콘으로 표현

## ERD 엔티티 관계 표기법

각 엔티티 유형을 만든 후 엔티티끼리 관계가 있으면 선을 이어 관계 맺어주기티비

실선 - 강한 관계 → 식별자 관계

점선 - 약하 관계 - 비식별자 관계

![식별자 관계](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%208.png)

식별자 관계

![비식별자 관계](ERD%20%E1%84%91%E1%85%AD%E1%84%80%E1%85%B5%E1%84%87%E1%85%A5%E1%86%B8%20731b256ae70043cc8a5b7a5040b426eb/img1.daumcdn%209.png)

비식별자 관계