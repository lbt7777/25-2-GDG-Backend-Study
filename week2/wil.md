# 2주차 과제 - wil.md

## 1. 2주차에 학습한 내용
- 계층형 아키텍쳐는 프론트엔드, 컨트롤러, 서비스, 레포지토리, DB로 역할이 분리되어 있다.
- Controller는 요청을 받고 진입점, Service는 비즈니스 로직을 처리하는 핵심 계층이다. 
- 레포지토리는 데이터 접근을 담당하고, DTO와 Entity를 구분해 데이터 전달과 저장 역할을 분리한다.
- Controller 계층에서는 HTTP요청을 받아 DTO형태로 데이터를 전달하고, 서비스 계층과 통신하여 결과를 응답하고 @Controller, @RestController, @RequestMapping, @RequestBody등을 사용해 엔드포인트를 구현한다. 또한 ResopnseEntity와 HTTP 상태 코드를 통해 명확한 응답을 설계할 수 있다.
- Service 계층에서는 실제 비즈니스 로직이 구현되며, 데이터 조회 및 수정, 트랜잭션 관리 등을 담당한다. 트랜잭션은 작업의 원자성을 보장하고, 오류 발생 시 롤백이 가능하도록 한다.
- 스프링 컨테이너(Application Context)느느 빈을 관리하며, 필요한 객체를 직접 생성하지 않고 외부에서 주입받는다. @ComponentScan, @Controller, @Service, @Repository 등을 통해 빈을 자동 등록하고, 생성자 주입(@Autowired 또는 @RequiredArgsConstructor)으로 안전하고 효율적인 의존성 관리가 가능하다.
- 패키지 구조는 기능별로 나누는 계층형 구조와 도메인 단위로 묶는 도메인형 구조를 비교했고 유지보수성과 확장성 측면에서 도메인형 구조가 실무에서 선호된다.
