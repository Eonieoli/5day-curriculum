# Python 응용 과정 커리큘럼 v5.0

## 📋 과정 개요

- **과정명**: Python 응용 과정
- **목표**: 웹 개념 이해 및 FastAPI로 REST API 개발
- **기간**: 5일 (Day 6 ~ Day 10)
- **일일 시간**: 8교시 (명목상 50분 × 8 = 400분, 실제 약 7시간)
- **총 시간**: 약 35시간
- **선수 과정**: Python 기초 과정 (Day 1-5)
- **휴식**: 각 교시 사이 10분, 점심 시간 1시간

## 🎯 교육 구조

### 5단계 학습 방법론

1. **개념 (Concept)**: 이론 설명, 정의, 필요성
2. **Basic (Example)**: 강사가 보여주는 예제 코드 (학생은 관찰)
3. **Practice (Guided)**: 강사와 함께 타이핑하며 익히기
4. **Exercise (Independent)**: 학생이 스스로 문제 풀기
5. **Problem (Comprehensive)**: 종합 실습 (8교시, 기초/응용/도전 3단계)

### 시간 배분 원칙

**일반 교시 (1-7교시, 50분)**

- 개념: 5-15분 (이론 중심 교시는 더 길게)
- Basic: 15-25분 (실습 중심 교시는 더 길게)
- Practice: 10-20분
- Exercise: 10-15분 (v4보다 확대!)

**8교시 종합 실습 (50분)**

- 복습 퀴즈: 10분
- 🟢 기초 Problem: 15분
- 🟡 응용 Problem: 15분
- 🔴 도전 Problem: 10분

**복습 교시 (매일 1교시, 50분)**

- 퀴즈: 20분
- 실습 복습: 25분
- Q&A: 5분

---

## Day 6: 웹과 API의 이해

### 1교시: 환경 구축 + 기초 복습 ⭐⭐

- **환경 구축 (25분)**:
  - 가상환경 생성 (`python -m venv venv`)
  - 활성화 (Git Bash: `source venv/Scripts/activate`)
  - FastAPI 설치 (`pip install fastapi uvicorn`)
  - 설치 확인 (`pip list`)
  - 간단한 테스트 (`import fastapi`)
  - 트러블슈팅 (개별 지도)
- **기초 복습 퀴즈 (20분)**:
  - 딕셔너리, 타입 힌트, 함수, import
- **응용 과정 소개 (5분)**:
  - 로드맵, 최종 목표 (REST API 구축)

> **중요**: 모든 학생이 동일한 환경! 문제 있으면 즉시 해결!

### 2교시: JSON 기초 ⭐⭐⭐

- **개념 (10분)**:
  - JSON이란? (JavaScript Object Notation)
  - 딕셔너리 ↔ 텍스트 변환
  - 왜 필요? (웹에서 데이터 주고받기)
  - FastAPI에서의 역할
- **Basic (22분)**:
  - 딕셔너리 → JSON: `json.dumps()`
    ```python
    import json
    user = {"name": "Alice", "age": 25}
    json_str = json.dumps(user, indent=2)
    ```
  - JSON → 딕셔너리: `json.loads()`
  - 파일 저장: `json.dump()`
  - 파일 로드: `json.load()`
  - with open() 패턴
- **Practice (11분)**:
  - 학생 정보 → JSON 저장
  - JSON 파일 읽기
  - 수정 후 다시 저장
- **Exercise (7분)**:
  - 상품 목록 JSON 관리

### 3교시: 웹의 동작 원리 ⭐⭐

- **개념 (12분)**:
  - 클라이언트-서버 모델
  - 브라우저 역할
  - IP/도메인/포트
  - URL 구조
- **Basic (18분)**:
  - 브라우저 개발자 도구 실습
  - 네트워크 탭 관찰
  - URL 파싱 예제
- **Practice (10분)**:
  - URL 분해하기
  - 쿼리 파라미터 이해
- **Exercise (10min)**:
  - URL 구조 분석 문제

### 4교시: HTTP 메서드와 상태 코드 ⭐⭐

- **개념 (10분)**:
  - HTTP란? Request/Response
  - HTTP 메서드 (GET, POST, PUT, DELETE)
  - 상태 코드 (2xx, 4xx, 5xx)
- **Basic (22분)**:
  - 각 메서드 시나리오
  - 주요 상태 코드 (200, 201, 400, 404, 500)
  - 개발자 도구로 관찰
  - Content-Type 헤더
- **Practice (10분)**:
  - 브라우저에서 GET 확인
  - 개발자 도구 실습
- **Exercise (8분)**:
  - 메서드/상태 코드 매칭

### 5교시: REST API 개념 ⭐⭐⭐

- **개념 (12분)**:
  - API란?
  - REST 아키텍처 원칙
  - RESTful API 설계
  - 리소스와 엔드포인트
- **Basic (20분)**:
  - 좋은 API vs 나쁜 API
  - 리소스 명명 규칙
  - HTTP 메서드 매핑
- **Practice (10분)**:
  - 블로그 API 설계 (함께)
- **Exercise (8분)**:
  - TODO 앱 API 설계

### 6교시: Postman 사용법 ⭐⭐

- **개념 (5min)**:
  - Postman이란?
  - API 테스팅 도구 필요성
- **설치 확인 (5분)**:
  - 설치 안 된 학생 다운로드
  - 간단한 소개
- **Basic (25분)**:
  - GET 요청
  - POST 요청
  - Headers 설정
  - Body 설정 (JSON)
  - 컬렉션
- **Practice (10분)**:
  - 공개 API 테스트 (JSONPlaceholder)
  - JSON 데이터 전송
- **Exercise (5분)**:
  - 특정 API 호출 과제

### 7교시: JSON + HTTP 통합 실습 ⭐⭐

- **개념 (5분)**:
  - HTTP Body
  - Request/Response에서 JSON 역할
- **Basic (20분)**:
  - 실제 API 응답 분석
  - JSON 파싱
  - 중첩 데이터 처리
- **Practice (13분)**:
  - 공개 API 응답 파싱
  - 데이터 추출 및 가공
- **Exercise (12분)**:
  - API 응답을 딕셔너리로
  - 필요한 정보만 추출

### 8교시: Day 6 종합 실습

- **복습 퀴즈 (10분)**: JSON, HTTP, REST, Postman
- **🟢 기초 Problem (15분)**: REST API 설계서 작성
- **🟡 응용 Problem (15분)**: Postman으로 공개 API 테스트 + JSON 가공
- **🔴 도전 Problem (10분)**: 복잡한 JSON 파싱

---

## Day 7: FastAPI 시작하기

### 1교시: Day 6 복습

- **퀴즈 (20분)**: JSON, HTTP, REST API, Postman
- **실습 복습 (25분)**: JSON 파일 읽기/쓰기, Postman 실습
- **Q&A (5분)**

### 2교시: FastAPI 소개 + 첫 API ⭐⭐⭐

- **개념 (10분)**:
  - FastAPI란?
  - 특징과 장점
  - 다른 프레임워크 비교
- **환경 확인 (5분)**: pip list로 설치 확인
- **Basic (20분)**:
  - Hello World API
  - uvicorn 실행
  - 브라우저 확인
  - --reload 옵션
- **Practice (10min)**:
  - 함께 첫 API 만들기
- **Exercise (5분)**:
  - 자기소개 API
  - 현재 시간 API

### 3교시: 자동 문서화 ⭐⭐⭐

- **개념 (7분)**:
  - Swagger UI
  - ReDoc
  - 자동 문서화 장점
- **Basic (20분)**:
  - /docs 접속
  - /redoc 접속
  - 문서에서 API 테스트
  - docstring 추가
- **Practice (13분)**:
  - 여러 API 만들고 문서 확인
  - 설명 추가
- **Exercise (10분)**:
  - 문서화가 잘 된 API 3개

### 4교시: 경로 매개변수 (Path Parameter) ⭐⭐⭐

- **개념 (8분)**:
  - 경로 매개변수란?
  - 동적 라우팅
  - 타입 지정
- **Basic (22분)**:
  - {item_id} 문법
  - int 타입, str 타입
  - 자동 검증
  - 에러 응답
- **Practice (10분)**:
  - 사용자 조회 API
  - 상품 조회 API
- **Exercise (10분)**:
  - 게시글 조회
  - 카테고리별 조회

### 5교시: 쿼리 매개변수 (Query Parameter) ⭐⭐⭐

- **개념 (8min)**:
  - 쿼리 매개변수란?
  - ?key=value 형식
  - 검색/필터링 용도
- **Basic (22분)**:
  - 기본 쿼리
  - 기본값 설정
  - Optional 쿼리
  - 여러 개 쿼리
- **Practice (10분)**:
  - 검색 API
  - 페이징 API (skip, limit)
- **Exercise (10분)**:
  - 필터링 API (여러 조건)

### 6교시: 경로 + 쿼리 조합 ⭐⭐

- **개념 (5분)**:
  - 경로와 쿼리 함께 사용
  - 우선순위
- **Basic (18분)**:
  - 조합 예제
  - 실전 API 패턴
  - Postman 테스트
- **Practice (15분)**:
  - 사용자의 게시글 조회
  - 상품 검색 API
- **Exercise (12min)**:
  - 복합 API 만들기

### 7교시: Response 모델 기초 ⭐⭐

- **개념 (8분)**:
  - 응답 구조
  - 딕셔너리 반환
  - 일관된 응답 구조
- **Basic (20분)**:
  - 간단한 Response 모델
  - dict 반환
  - 일관된 응답 구조
  - JSON 응답 확인
- **Practice (12분)**:
  - 사용자 응답
  - 상품 응답
- **Exercise (10분)**:
  - 응답 모델 설계

### 8교시: Day 7 종합 실습

- **복습 퀴즈 (10분)**: FastAPI 기본, 경로/쿼리 매개변수
- **🟢 기초 Problem (15분)**: 간단한 도서관 API (책 조회)
- **🟡 응용 Problem (15분)**: 쇼핑몰 상품 API (경로+쿼리)
- **🔴 도전 Problem (10분)**: 복잡한 검색 API

---

## Day 8: Pydantic과 Request/Response

### 1교시: Day 7 복습

- **퀴즈 (20분)**: FastAPI 기본, 매개변수
- **실습 복습 (25분)**: 경로/쿼리 매개변수 재실습
- **Q&A (5분)**

### 2교시: Pydantic 모델 기초 ⭐⭐⭐

- **개념 (10분)**:
  - Pydantic이란?
  - BaseModel
  - 자동 검증
  - FastAPI에서의 역할
- **Basic (22분)**:
  - BaseModel 상속
  - 필드 정의
  - 인스턴스 생성
  - 자동 타입 변환
- **Practice (10분)**:
  - User 모델
  - Product 모델
- **Exercise (8min)**:
  - Post 모델
  - Comment 모델

### 3교시: Request Body ⭐⭐⭐

- **개념 (8분)**:
  - Request Body란?
  - POST/PUT에서 사용
  - JSON과의 관계
- **Basic (22분)**:
  - POST 엔드포인트
  - Pydantic 모델로 받기
  - 자동 검증
  - 에러 응답 (422)
- **Practice (10분)**:
  - 사용자 생성 API
  - 상품 등록 API
- **Exercise (10분)**:
  - 게시글 작성 API

### 4교시: Pydantic 검증 기능 ⭐⭐⭐

- **개념 (12분)**:
  - Field() 함수
  - 검증 규칙
  - 에러 메시지
  - 보안
- **Basic (20min)**:
  - 최소/최대값
  - 길이 제한
  - 정규식
  - 커스텀 검증
- **Practice (10분)**:
  - 회원가입 모델 (이메일, 비밀번호)
- **Exercise (8분)**:
  - 상품 등록 검증

### 5교시: Response Model ⭐⭐

- **개념 (8min)**:
  - response_model이란?
  - 응답 데이터 제어
  - 민감정보 제외
- **Basic (20분)**:
  - response_model 지정
  - 비밀번호 제외
  - List[Model] 반환
- **Practice (12분)**:
  - 사용자 조회 (비밀번호 제외)
  - 목록 조회
- **Exercise (10분)**:
  - 안전한 응답 모델

### 6교시: 상태 코드 지정 ⭐⭐

- **개념 (8분)**:
  - status_code 매개변수
  - HTTPException
  - 적절한 상태 코드 선택
- **Basic (20분)**:
  - 201 Created
  - 400 Bad Request
  - 404 Not Found
  - HTTPException 사용
- **Practice (12분)**:
  - CRUD API에 상태 코드 적용
- **Exercise (10분)**:
  - 에러 핸들링이 있는 API

### 7교시: Optional과 Union 활용 ⭐⭐

- **개념 (8분)**:
  - Optional 필드
  - 부분 업데이트
  - Union 타입
- **Basic (20분)**:
  - Optional[str]
  - None 기본값
  - PATCH 메서드
  - 선택적 필드
- **Practice (12분)**:
  - 프로필 업데이트 API
- **Exercise (10min)**:
  - 유연한 업데이트 API

### 8교시: Day 8 종합 실습

- **복습 퀴즈 (10분)**: Pydantic, Request/Response
- **🟢 기초 Problem (15분)**: TODO API (CRUD 기본)
- **🟡 응용 Problem (15분)**: 블로그 API (검증 포함)
- **🔴 도전 Problem (10분)**: 복잡한 검증 규칙

---

## Day 9: 데이터베이스 연동

### 1교시: Day 8 복습

- **퀴즈 (20분)**: Pydantic 전체
- **실습 복습 (25분)**: Request Body, 검증
- **Q&A (5분)**

### 2교시: 데이터베이스 기초 + SQLite ⭐⭐

- **개념 (15분)**:
  - 데이터베이스란?
  - RDBMS
  - SQLite 특징
  - 테이블/행/열
- **Basic (22분)**:
  - SQL 기본 (SELECT, INSERT, UPDATE, DELETE)
  - SQLite 브라우저
- **Practice (8분)**:
  - SQL 문법 연습
- **Exercise (5분)**:
  - 기본 SQL 작성

### 3교시: SQLite 연결 ⭐⭐

- **개념 (8분)**:
  - sqlite3 모듈
  - 커넥션과 커서
  - commit의 중요성
- **Basic (22분)**:
  - 데이터베이스 연결
  - 테이블 생성
  - 커서 사용
  - 커넥션 닫기
- **Practice (10min)**:
  - 데이터베이스 초기화
- **Exercise (10분)**:
  - 테이블 설계 및 생성

### 4교시: 데이터 삽입 (CREATE) ⭐⭐

- **개념 (10분)**:
  - INSERT문
  - 파라미터 바인딩
  - SQL Injection 방지
- **Basic (20분)**:
  - 단일 삽입
  - 여러 개 삽입
  - executemany()
  - lastrowid
- **Practice (10분)**:
  - 사용자 추가 함수
  - 상품 추가 함수
- **Exercise (10min)**:
  - 데이터 삽입 API

### 5교시: 데이터 조회 (READ) ⭐⭐⭐

- **개념 (7분)**:
  - SELECT문
  - WHERE 조건
  - fetchone/fetchall
- **Basic (22분)**:
  - 전체 조회
  - 조건 조회
  - 단일 조회
  - 컬럼 선택
- **Practice (11분)**:
  - 목록 조회 함수
  - 상세 조회 함수
- **Exercise (10분)**:
  - 조건별 조회 API

### 6교시: 데이터 수정 및 삭제 (UPDATE, DELETE) ⭐⭐

- **개념 (7분)**:
  - UPDATE문
  - DELETE문
  - WHERE의 중요성
- **Basic (20분)**:
  - 수정
  - 삭제
  - 안전한 삭제 (존재 확인)
- **Practice (13min)**:
  - 업데이트 함수
  - 삭제 함수
- **Exercise (10분)**:
  - 수정/삭제 API

### 7교시: FastAPI + SQLite 통합 ⭐⭐⭐

- **개념 (10분)**:
  - 엔드포인트에서 DB 작업
  - 함수 분리
  - 에러 처리
- **Basic (22분)**:
  - CRUD API 전체 구현
  - Pydantic + DB 조합
  - 트랜잭션
- **Practice (10분)**:
  - 완전한 게시판 API
- **Exercise (8min)**:
  - TODO API에 DB 적용

### 8교시: Day 9 종합 실습

- **복습 퀴즈 (10분)**: SQL, SQLite, CRUD
- **🟢 기초 Problem (15분)**: 간단한 메모 API (DB 포함)
- **🟡 응용 Problem (15분)**: 사용자 관리 시스템
- **🔴 도전 Problem (10분)**: 검색 기능 추가

---

## Day 10: REST API 설계 및 프로젝트

### 1교시: Day 9 복습

- **퀴즈 (20분)**: 데이터베이스, CRUD
- **실습 복습 (25분)**: FastAPI + DB 통합
- **Q&A (5분)**

### 2교시: REST API 설계 실습 ⭐⭐⭐

- **개념 (10분)**:
  - RESTful 설계 원칙 복습
  - 엔드포인트 네이밍
  - HTTP 메서드 선택
- **Basic (20분)**:
  - 좋은 설계 vs 나쁜 설계
  - 실제 서비스 API 분석
- **Practice (12분)**:
  - 도서관 시스템 API 설계
- **Exercise (8분)**:
  - 쇼핑몰 API 설계

### 3교시: 라우터 분리 ⭐⭐

- **개념 (8min)**:
  - APIRouter
  - 코드 구조화
  - 관심사 분리
- **Basic (20분)**:
  - APIRouter 사용
  - prefix 설정
  - tags
  - include_router
- **Practice (12분)**:
  - users, posts 라우터 분리
- **Exercise (10분)**:
  - 3개 이상 라우터 구성

### 4교시: 에러 처리 고도화 ⭐⭐

- **개념 (8분)**:
  - HTTPException 심화
  - 커스텀 에러
  - 일관된 에러 응답
- **Basic (20분)**:
  - 404 Not Found
  - 400 Bad Request
  - 상세 에러 메시지
  - detail 활용
- **Practice (12분)**:
  - 에러 핸들링 함수
- **Exercise (10분)**:
  - 모든 API에 에러 처리

### 5교시: 페이지네이션 + 프로젝트 준비 ⭐⭐

- **페이지네이션 (30분)**:
  - **개념 (7min)**: 필요성, skip/limit 패턴
  - **Basic (15분)**:
    - skip, limit 받기
    - SQL LIMIT/OFFSET
    - 전체 개수 반환
  - **Practice (8분)**: 페이지네이션 구현
- **프로젝트 주제 선정 (20분)**:
  - 주제 소개 (TODO, 블로그, 쇼핑몰, 게시판)
  - 팀/개인 결정
  - 주제 확정

### 6교시: 프로젝트 설계 ⭐⭐⭐

- **요구사항 정의 (20분)**:
  - 기능 목록 작성
  - 우선순위 결정 (MVP)
  - 필수 vs 선택 기능
- **API 스펙 작성 (20분)**:
  - 엔드포인트 설계
  - Request/Response 모델
  - HTTP 메서드 매핑
- **DB 스키마 설계 (10분)**:
  - 테이블 구조
  - 필드 정의

### 7교시: 프로젝트 구현 (1) ⭐⭐⭐

- **초기 설정 (15분)**:
  - 디렉터리 구조
  - DB 초기화
  - Pydantic 모델 작성
- **핵심 CRUD (35분)**:
  - 핵심 엔드포인트 구현
  - DB 연동
  - 기본 검증

### 8교시: 프로젝트 구현 (2) + 발표 ⭐⭐⭐

- **기능 완성 (25분)**:
  - 추가 엔드포인트
  - 에러 처리
  - 검증 강화
  - Postman 테스트
- **간단한 발표 (20분)**:
  - 3-4팀 간단한 시연 (각 5분)
  - 주요 기능 소개
  - 배운 점 공유
- **회고 (5분)**:
  - 전체 소감
  - 아쉬운 점

> **참고**: 완성도보다 경험 중심! 학습 과정이 중요!

---

## 📌 핵심 학습 목표 (FastAPI 중심)

### 최우선 항목 ⭐⭐⭐

1. **JSON**: 딕셔너리 ↔ 텍스트, 웹 데이터 교환
2. **Pydantic 모델**: Request/Response 구조화
3. **경로/쿼리 매개변수**: API 엔드포인트 설계
4. **CRUD 작업**: 데이터베이스 연동
5. **REST API 설계**: RESTful 원칙 적용
6. **에러 처리**: HTTPException, 상태 코드
7. **Postman**: API 테스팅

### 중요 항목 ⭐⭐

1. HTTP 프로토콜 이해
2. SQLite 기본
3. 라우터 분리
4. 페이지네이션

### 기본 항목 ⭐

1. 웹 동작 원리
2. 자동 문서화
3. SQL 기본 문법

---
