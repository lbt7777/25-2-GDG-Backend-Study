# 1주차 과제

## 1. 1주차에 학습한 내용
이번 주차에서는 웹의 기본 개념과 동작 방식, 그리고 HTTP 및 REST API에 대해 학습했다. 웹은 인터넷 위에서 동작하는 서비스이며, 클라이언트와 서버가 요청(Request)과 응답(Response)을 통해 통신한다. URL은 스킴(프로토콜), 호스트, 포트, 경로, 쿼리로 구성되며, 이를 통해 특정 자원을 식별한다. HTTP는 무상태성(Stateless)과 비연결성(Connectionless)을 특징으로 하며, 요청과 응답을 기반으로 동작한다. HTTP 요청은 Start line, Header, Body로 구성되고, 응답은 Status line, Header, Body로 구성된다. 주요 HTTP 메서드에는 GET(조회), POST(등록), PUT(수정 및 생성), PATCH(일부 수정), DELETE(삭제)가 있다. 상태 코드는 200(성공), 201(생성), 400(잘못된 요청), 404(리소스 없음), 500(서버 오류) 등이 있다. REST API는 자원(Resource), 행위(Verb), 표현(Representation)을 기반으로 설계되며, HTTP 메서드와 URI를 이용해 자원을 식별하고 조작한다. 회원 등록, 조회, 수정, 삭제 기능을 설계하는 예시를 통해 RESTful한 API 설계 방식을 학습했다. 또한 프론트엔드와 백엔드의 역할 분리, 데이터베이스를 통한 정보 저장 및 관리 개념을 정리했다.

## 2. Spring Boot 애플리케이션을 실행하고, 브라우저에 localhost:8080 을 입력했을 때 나오는 Whitelabel Error Page 스크린샷
<img width="682" height="278" alt="whitelabel error page" src="https://github.com/user-attachments/assets/1c436218-0421-4ac4-8089-08513e67ef34" />

## 3. 온라인 쇼핑몰 프로젝트 API 명세서 작성
- 상품 기능
  - 상품 정보 등록 HTTP Method : POST, URL : /products
  - 상품 목록 조회 HTTP Method : GET, URL : /products
  - 개별 상품 정보 상세 조회 HTTP Method : GET, URL : /products/{productId}
  - 상품 정보 수정 HTTP Method : PATCH, URL : /products/{productId}
  - 상품 삭제 HTTP Method : DELETE, URL : /products/{productId}

- 주문 기능
  - 주문 정보 생성 HTTP Method : POST, URL : /orders
  - 주문 목록 조회 HTTP Method : GET, URL : /orders
  - 개별 주문 정보 상세 조회 HTTP Method : GET, URL : /orders/{orderId}
  - 주문 취소 HTTP Method : POST, URL : /orders/{orderId}/cancel
