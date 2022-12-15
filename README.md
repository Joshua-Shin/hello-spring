## Spring을 활용한 웹 백엔드 개발 프로젝트
  - 본 프로젝트는 <스프링 입문 - 김영한> 강의를 수강하며 진행한 실습 프로젝트 입니다.

--------------------

## 강의 내용 자유 회상

### 1. Static, 웹 MVC, API  
- static은 html 그대로 웹 브라우저에 띄워주는거  
- 웹 MVC는 model, view, controller 를 통해 template에 있는 리소스와 동적으로 동작하여 웹 브라우저에 띄워주는거  
- API는 json 형식으로 데이터를 바로 전달해주는거  

### 2. 전체 구조는 Controller, Service, Repository
- 연동 방식에는 두가지
- 컴포넌트 스캔 자동 연동.
- 직접 자바 코드로 config 작성해서 연동 
- DI. 방식으로는 3가지
- 생성자 주입, 필드 주입, setter 주입.
- 보통은 생성자 주입 사용.

### 3. DB와 연동하는 방식
- 순수 jdbc,
- jdbc template
- JPA
- 스프링 데이터 JPA
- 쿼리를 직접 짜는걸 줄이는 형태로 발전.
- JPA부터 쿼리를 직접 짜지 않고 객체 형태로 DB에게 쿼리를 넘겨주게됨.
- 물론 완전하게 쿼리를 아예 안짤수는 없어.
- 스프링 데이터 JPA는 여러 메소드들을 다 구현해줘서 DB와 훨씬 더 편하게 쿼리 전달 가능.

### 4. AOP
- 핵심 관심사항과 공통 관심 사항을 분리해줘야 돼.
- 여기에서는 공통 관심 사항으로 시간측정 하는걸 둠.
- 스프링 컨테이너에 있는 스프링 빈에 하나하나 붙이는게 아니라,
- 공통 관심 사항을 하나의 스프링 빈으로 만들어서, 원하는 빈에다가 붙여서 사용.
- 사실은 프록시를 만들어서 거기에 붙어서 작용하고 origin 빈을 다시 작동시켜 진행함.




