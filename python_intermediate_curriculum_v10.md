# Python 응용 과정 커리큘럼 v10.0

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
- Exercise: 10-15분

**8교시 종합 실습 (50분)**

- 복습 퀴즈: 10분
- 🟢 기초 Problem: 15분
- 🟡 응용 Problem: 15분
- 🔴 도전 Problem: 10분

**복습 교시 (매일 1교시, 50분)**

- 복습 퀴즈: 10분 (간소화!)
- 핵심 복습: 15분 (전날 가장 중요한 것만!)
- 새 내용: 25분 (바로 진도!)

---

## Day 6: 웹과 API의 이해

### 1교시: 복습 + JSON/with문 시작 ⭐⭐⭐ (수정!)

- **복습 퀴즈 (10min)**: Python 기초 핵심 (딕셔너리, 타입 힌트, 함수)
- **핵심 복습 (10min)**:
  - 딕셔너리 복습 (JSON의 기초!)
  - 타입 힌트 복습
  - 간단한 Q&A
- **JSON + with문 시작 (30min)**:
  - 개념 (10min):
    - with문이란? 자동 close
    - JSON이란? 딕셔너리 ↔ 텍스트
    - 웹에서 데이터 주고받기
    - FastAPI에서의 역할
  - Basic (20min):
    - with open() 기본: `with open('file.json', 'r') as f:`
    - JSON 메모리 변환 시작: `json.dumps()`, `json.loads()`

> **중요 변경**: 환경 구축 제거! Day 7로 이동!

### 2교시: JSON 기초 + with문 ⭐⭐⭐

- **Basic 완성 (22min)**:
  - JSON 메모리 변환 완성 (8min):

    ```python
    import json

    user = {"name": "Alice", "age": 25}

    # 딕셔너리 → JSON 문자열
    json_str = json.dumps(user, indent=2)

    # JSON 문자열 → 딕셔너리
    user_dict = json.loads(json_str)
    ```

  - JSON 파일 입출력 (14min):

    ```python
    # 저장
    with open('user.json', 'w') as f:
        json.dump(user, f, indent=2)

    # 로드
    with open('user.json', 'r') as f:
        user = json.load(f)

    # 실전 예제: 설정 파일, 데이터 저장
    ```
- **Practice (18min)**:
  - 학생 정보 딕셔너리 → JSON 파일 저장
  - JSON 파일 읽기 → 딕셔너리로 변환
  - 데이터 수정 → 다시 JSON 저장
- **Exercise (10min)**:
  - 상품 목록 JSON 관리
    - 상품 추가
    - 목록 조회
    - 가격 수정

> **중요**: with문을 실제로 써먹으면서 배움!

### 3교시: 웹의 동작 원리 ⭐⭐

- **개념 (10분)**:
  - 클라이언트-서버 모델
  - 브라우저 역할
  - URL 구조 (간단히)

- **Basic (15분)**:
  - 브라우저 개발자 도구 실습
  - 네트워크 탭 관찰
  - URL 파싱 예제

- **Practice (15분)**:
  - URL 분해하기
  - 쿼리 파라미터 이해
  - 개발자 도구로 요청 확인

- **Exercise (10분)**:
  - URL 구조 분석 문제

> IP, 도메인, 포트 세부 내용 축소
> 개발자 도구 실습에 집중

### 4교시: HTTP 메서드와 상태 코드 ⭐⭐

- **개념 (10min)**:
  - HTTP란? Request/Response
  - HTTP 메서드 (GET, POST, PUT, DELETE)
  - 상태 코드 (2xx, 4xx, 5xx)
- **Basic (22min)**:
  - 각 메서드 시나리오
  - 주요 상태 코드 (200, 201, 400, 404, 500)
  - 개발자 도구로 관찰
  - Content-Type 헤더
- **Practice (10min)**:
  - 브라우저에서 GET 확인
  - 개발자 도구 실습
- **Exercise (8min)**:
  - 메서드/상태 코드 매칭

### 5교시: REST API 개념 ⭐⭐⭐

- **개념 (12min)**:
  - API란?
  - REST 아키텍처 원칙
  - RESTful API 설계
  - 리소스와 엔드포인트
- **Basic (20min)**:
  - 좋은 API vs 나쁜 API
  - 리소스 명명 규칙
  - HTTP 메서드 매핑
- **Practice (10min)**:
  - 블로그 API 설계 (함께)
- **Exercise (8min)**:
  - TODO 앱 API 설계

### 6교시: Postman 사용법 ⭐⭐

- **개념 (5min)**:
  - Postman이란?
  - API 테스팅 도구 필요성
- **설치 확인 (5min)**:
  - 설치 안 된 학생 다운로드
  - 간단한 소개
- **Basic (25min)**:
  - GET 요청
  - POST 요청
  - Headers 설정
  - Body 설정 (JSON)
  - 컬렉션
- **Practice (10min)**:
  - 공개 API 테스트 (JSONPlaceholder)
  - JSON 데이터 전송
- **Exercise (5min)**:
  - 특정 API 호출 과제

### 7교시: JSON + HTTP 통합 실습 ⭐⭐

- **개념 (5min)**:
  - HTTP Body
  - Request/Response에서 JSON 역할
- **Basic (20min)**:
  - 실제 API 응답 분석
  - JSON 파싱
  - 중첩 데이터 처리
- **Practice (13min)**:
  - 공개 API 응답 파싱
  - 데이터 추출 및 가공
- **Exercise (12min)**:
  - API 응답을 딕셔너리로
  - 필요한 정보만 추출

### 8교시: Day 6 종합 실습

- **복습 퀴즈 (10min)**: JSON, HTTP, REST, Postman
- **🟢 기초 Problem (15min)**: REST API 설계서 작성
- **🟡 응용 Problem (15min)**: Postman으로 공개 API 테스트 + JSON 가공
- **🔴 도전 Problem (10min)**: 복잡한 JSON 파싱

---

## Day 7: FastAPI 시작하기

### 1교시: Day 6 복습 + 환경 구축 + FastAPI 시작 ⭐⭐⭐ (수정!)

- **복습 퀴즈 (5min)**: JSON, HTTP, REST (짧게!)
- **환경 구축 (30min)**: ← Day 6에서 이동!
  - 가상환경 생성 (10min):
    - `python -m venv venv`
    - 개념 설명: 왜 가상환경이 필요한가?
  - 활성화 (5min):
    - Windows: `venv\Scripts\activate`
    - Git Bash: `source venv/Scripts/activate`
    - Mac/Linux: `source venv/bin/activate`
  - FastAPI 설치 (10min):
    - `pip install fastapi uvicorn`
    - 설치 확인 (`pip list`)
    - 버전 확인
  - 테스트 (5min):
    - `import fastapi` 테스트
    - 간단한 코드 실행
- **FastAPI 소개 (15min)**:
  - FastAPI란?
  - 특징과 장점
  - 다른 프레임워크 비교
  - Hello World 준비

> **중요 변경**: 환경 구축을 Day 6에서 이동!
> → 설치하자마자 바로 사용!

### 2교시: FastAPI 첫 API + 자동 문서화 ⭐⭐⭐ (수정!)

- **FastAPI 첫 API (30min)**:
  - **Basic (20min)**:
    - Hello World API 완성
    - uvicorn 실행
    - 브라우저 확인
    - --reload 옵션
    - 여러 엔드포인트 추가
  - **Practice (10min)**:
    - 함께 첫 API 만들기
    - 자기소개 API
    - 간단한 계산 API

- **자동 문서화 (20min)**:
  - 개념 (5min):
    - Swagger UI
    - ReDoc
    - 자동 문서화 장점
  - Basic (10min):
    - /docs 접속
    - /redoc 접속
    - 문서에서 API 테스트
    - docstring 추가
  - Practice (5min):
    - 여러 API 만들고 문서 확인

> **중요 변경**: requests 제거! Day 10으로 이동!
> → FastAPI + 문서화에 집중!

### 3교시: 자동 문서화 심화 ⭐⭐⭐

- **Basic (20min)**:
  - 설명 추가
  - 태그 추가
  - 문서 커스터마이징
  - 실전 예제
- **Practice (20min)**:
  - 여러 API 만들고 문서 확인
  - 설명 추가
  - 태그로 그룹화
- **Exercise (10min)**:
  - 문서화가 잘 된 API 3개

### 4교시: 경로 매개변수 (Path Parameter) ⭐⭐⭐

- **개념 (8min)**:
  - 경로 매개변수란?
  - 동적 라우팅
  - 타입 지정
- **Basic (22min)**:
  - {item_id} 문법
  - int 타입, str 타입
  - 자동 검증
  - 에러 응답
- **Practice (10min)**:
  - 사용자 조회 API
  - 상품 조회 API
- **Exercise (10min)**:
  - 게시글 조회
  - 카테고리별 조회

### 5교시: 쿼리 매개변수 (Query Parameter) ⭐⭐⭐

- **개념 (8min)**:
  - 쿼리 매개변수란?
  - ?key=value 형식
  - 검색/필터링 용도
- **Basic (22min)**:
  - 기본 쿼리
  - 기본값 설정
  - Optional 쿼리
  - 여러 개 쿼리
- **Practice (10min)**:
  - 검색 API
  - 페이징 API (skip, limit)
- **Exercise (10min)**:
  - 필터링 API (여러 조건)

### 6교시: 경로 + 쿼리 조합 ⭐⭐

- **개념 (5min)**:
  - 경로와 쿼리 함께 사용
  - 우선순위
- **Basic (18min)**:
  - 조합 예제
  - 실전 API 패턴
  - Postman 테스트
- **Practice (15min)**:
  - 사용자의 게시글 조회
  - 상품 검색 API
- **Exercise (12min)**:
  - 복합 API 만들기

### 7교시: 종합 실습 - 경로+쿼리 조합 ⭐⭐

- **개념 (5min)**: 실전 API 패턴 복습
- **Basic (15min)**:
  - 복합 엔드포인트 설계
  - 실전 예제 (사용자의 게시글)
  - Postman 테스트 전략
- **Practice (20min)**:
  - 상품 검색 API (카테고리+가격+정렬)
  - 사용자 프로필 + 활동 내역
  - 페이지네이션 기본 (skip/limit)
- **Exercise (10min)**:
  - 복잡한 검색 API
  - 여러 필터 조합

> **중요 변경**: Response 모델 제거! Day 8에서 Pydantic과 함께 배움!
> → 경로+쿼리 조합에 집중!

### 8교시: Day 7 종합 실습

- **복습 퀴즈 (10min)**: FastAPI 기본, 경로/쿼리 매개변수
- **🟢 기초 Problem (15min)**: 간단한 도서관 API (책 조회)
- **🟡 응용 Problem (15min)**: 쇼핑몰 상품 API (경로+쿼리)
- **🔴 도전 Problem (10min)**: 복잡한 필터링 API

---

## Day 8: Pydantic과 Request/Response

### 1교시: Day 7 복습 + Pydantic 시작

- **복습 퀴즈 (10min)**: FastAPI 기본, 매개변수
- **핵심 복습 (15min)**:
  - 경로/쿼리 매개변수 복습
  - 자동 문서 확인
  - 간단한 Q&A
- **Pydantic 기초 시작 (25min)**:
  - 개념 (10min):
    - Pydantic이란?
    - BaseModel
    - 자동 검증
    - FastAPI에서의 역할
  - Basic (15min):
    - BaseModel 상속
    - 필드 정의
    - 인스턴스 생성

### 2교시: Pydantic + Request/Response 통합 ⭐⭐⭐

- **Pydantic 기초 완성 (15min)**:
  - Basic (7min): 자동 타입 변환 예제
  - Practice (5min): User, Product 모델
  - Exercise (3min): Post, Comment 모델

- **Request Body (15min)**:
  - 개념 (3min): POST/PUT, JSON 매핑
  - Basic (8min):
    - POST 엔드포인트
    - Pydantic 모델로 받기
    - 자동 검증
    - 에러 응답 (422)
  - Practice (4min): 사용자 생성 API

- **Response Model (15min)**:
  - 개념 (3min): response_model, 민감정보 제외
  - Basic (8min):
    - response_model 지정
    - 비밀번호 제외 패턴
    - List[Model] 반환
  - Practice (4min): 안전한 응답

- **통합 예제 (5min)**:
  - 회원가입 API (Request + Response)

> **중요 개선**: Pydantic, Request, Response를 하나로 통합!
> → 흐름이 자연스럽고 이해 쉬움!

### 3교시: Request Body 심화 ⭐⭐⭐

- **개념 (8min)**:
  - 복잡한 Request Body
  - 여러 모델 조합
  - 실전 패턴
- **Basic (22min)**:
  - 중첩 모델
  - 리스트 필드
  - 선택적 필드
  - 실전 예제
- **Practice (12min)**:
  - 상품 등록 API (복잡한 구조)
  - 주문 API (여러 상품)
- **Exercise (8min)**:
  - 게시글 작성 API (태그, 카테고리 포함)

### 4교시: Pydantic 검증 + Validator ⭐⭐⭐

- **Field 검증 (30min)**:
  - 개념 (7min):
    - Field() 함수
    - 검증 규칙
    - 에러 메시지
    - 보안
  - Basic (15min):
    - 최소/최대값
    - 길이 제한
    - 정규식
    - 기본값
  - Practice (5min): 회원가입 모델 (이메일, 비밀번호)
  - Exercise (3min): 상품 등록 검증

- **Pydantic Validator (20min)**:
  - 개념 (5min): 커스텀 검증의 필요성
  - Basic (10min):

    ```python
    from pydantic import BaseModel, validator

    class User(BaseModel):
        email: str
        password: str

        @validator('email')
        def email_must_contain_at(cls, v):
            if '@' not in v:
                raise ValueError('Invalid email')
            return v.lower()  # 소문자로 변환

        @validator('password')
        def password_strength(cls, v):
            if len(v) < 8:
                raise ValueError('Password too short')
            if not any(c.isupper() for c in v):
                raise ValueError('Password must contain uppercase')
            return v
    ```

  - Practice (3min): 복잡한 검증 규칙
  - Exercise (2min): 커스텀 validator 작성

> **중요 추가**: Validator로 프로덕션 레벨 검증!

### 5교시: Response Model 심화 ⭐⭐

- **개념 (8min)**:
  - response_model 심화
  - 응답 데이터 제어
  - 성능 최적화
- **Basic (20min)**:
  - 선택적 필드 제거
  - response_model_exclude
  - response_model_include
  - List[Model] 심화
- **Practice (12min)**:
  - 사용자 목록 (비밀번호 제외)
  - 상품 목록 (재고 제외)
- **Exercise (10min)**:
  - 안전한 응답 모델 설계

### 6교시: 상태 코드 지정 ⭐⭐

- **개념 (8min)**:
  - status_code 매개변수
  - HTTPException
  - 적절한 상태 코드 선택
- **Basic (20min)**:
  - 201 Created
  - 400 Bad Request
  - 404 Not Found
  - HTTPException 사용
- **Practice (12min)**:
  - CRUD API에 상태 코드 적용
- **Exercise (10min)**:
  - 에러 핸들링이 있는 API

### 7교시: Optional과 Union 활용 ⭐⭐

- **개념 (8min)**:
  - Optional 필드
  - 부분 업데이트
  - Union 타입
- **Basic (20min)**:
  - Optional[str]
  - None 기본값
  - PATCH 메서드
  - 선택적 필드
- **Practice (12min)**:
  - 프로필 업데이트 API
- **Exercise (10min)**:
  - 유연한 업데이트 API

### 8교시: Day 8 종합 실습

- **복습 퀴즈 (10min)**: Pydantic, Request/Response, Validator
- **🟢 기초 Problem (15min)**: TODO API (CRUD 기본 + 검증)
- **🟡 응용 Problem (15min)**: 블로그 API (Validator 포함)
- **🔴 도전 Problem (10min)**: 복잡한 검증 규칙

---

## Day 9: 데이터베이스 연동

### 1교시: Day 8 복습 + DB 기초 시작

- **복습 퀴즈 (10min)**: Pydantic 전체, Validator
- **핵심 복습 (15min)**:
  - Request Body 복습
  - Validator 복습
  - 간단한 Q&A
- **DB 기초 시작 (25min)**:
  - 개념 (15min):
    - 데이터베이스란?
    - RDBMS
    - SQLite 특징
    - 테이블/행/열
  - Basic (10min):
    - SQL 기본 개념
    - SQLite 브라우저 소개

### 2교시: 데이터베이스 기초 + SQLite ⭐⭐

- **SQL 기본 (30min)**:
  - Basic (22min):
    - SELECT, INSERT, UPDATE, DELETE
    - WHERE 조건
    - 간단한 예제
  - Practice (8min): SQL 문법 연습
- **SQLite 브라우저 (20min)**:
  - 설치 확인
  - 테이블 생성 실습
  - 데이터 입력/조회

### 3교시: SQLite 연결 ⭐⭐

- **개념 (8min)**:
  - sqlite3 모듈
  - 커넥션과 커서
  - commit의 중요성
- **Basic (22min)**:
  - 데이터베이스 연결
  - 테이블 생성
  - 커서 사용
  - 커넥션 닫기
- **Practice (10min)**:
  - 데이터베이스 초기화
- **Exercise (10min)**:
  - 테이블 설계 및 생성

### 4교시: 데이터 삽입 (CREATE) ⭐⭐

- **개념 (10min)**:
  - INSERT문
  - 파라미터 바인딩
  - SQL Injection 방지
- **Basic (20min)**:
  - 단일 삽입
  - 여러 개 삽입
  - executemany()
  - lastrowid
- **Practice (10min)**:
  - 사용자 추가 함수
  - 상품 추가 함수
- **Exercise (10min)**:
  - 데이터 삽입 API

### 5교시: 데이터 조회 (READ) ⭐⭐⭐

- **개념 (7min)**:
  - SELECT문
  - WHERE 조건
  - fetchone/fetchall
- **Basic (22min)**:
  - 전체 조회
  - 조건 조회
  - 단일 조회
  - 컬럼 선택
- **Practice (11min)**:
  - 목록 조회 함수
  - 상세 조회 함수
- **Exercise (10min)**:
  - 조건별 조회 API

### 6교시: 데이터 수정 및 삭제 (UPDATE, DELETE) ⭐⭐

- **개념 (7min)**:
  - UPDATE문
  - DELETE문
  - WHERE의 중요성
- **Basic (20min)**:
  - 수정
  - 삭제
  - 안전한 삭제 (존재 확인)
- **Practice (13min)**:
  - 업데이트 함수
  - 삭제 함수
- **Exercise (10min)**:
  - 수정/삭제 API

### 7교시: FastAPI + SQLite 통합 + JOIN 기초 ⭐⭐⭐

- **FastAPI + SQLite 통합 (25min)**:
  - 개념 (5min): 엔드포인트에서 DB 작업
  - Basic (12min):
    - CRUD API 전체 구현
    - Pydantic + DB 조합
  - Practice (5min): 간단한 게시판 API
  - Exercise (3min): TODO API에 DB 적용

- **SQL JOIN 기초 (25min)**:
  - **개념 (8min)**:
    - 왜 필요한가? (단일 테이블의 한계)
    - 1:N 관계 (users - posts)
    - Foreign Key 개념
  - **Basic (12min)**:

    ```sql
    -- users 테이블
    CREATE TABLE users (
        id INTEGER PRIMARY KEY,
        name TEXT,
        email TEXT
    );

    -- posts 테이블 (user_id가 Foreign Key!)
    CREATE TABLE posts (
        id INTEGER PRIMARY KEY,
        title TEXT,
        content TEXT,
        user_id INTEGER,
        FOREIGN KEY (user_id) REFERENCES users(id)
    );

    -- INNER JOIN으로 게시글 + 작성자 정보
    SELECT posts.*, users.name, users.email
    FROM posts
    INNER JOIN users ON posts.user_id = users.id;

    -- 특정 사용자의 게시글만
    SELECT * FROM posts
    WHERE user_id = 1;
    ```

  - **Practice (3min)**:
    - 사용자-게시글 JOIN 쿼리
  - **Exercise (2min)**:
    - 댓글-작성자 JOIN

> **중요**: SQL JOIN으로 실무 DB 구조 이해!

### 8교시: Day 9 종합 실습

- **복습 퀴즈 (10min)**: SQL, SQLite, CRUD, JOIN
- **🟢 기초 Problem (15min)**: 간단한 메모 API (DB 포함)
- **🟡 응용 Problem (15min)**: 사용자 관리 시스템 (관계 포함)
- **🔴 도전 Problem (10min)**: JOIN을 활용한 복합 조회

---

## Day 10: REST API 설계 및 프로젝트

### 1교시: Day 9 복습 + REST 설계 시작

- **복습 퀴즈 (10min)**: 데이터베이스, CRUD, JOIN
- **핵심 복습 (15min)**:
  - FastAPI + DB 통합 복습
  - SQL JOIN 복습
  - 간단한 Q&A
- **REST 설계 시작 (25min)**:
  - 개념 (10min):
    - RESTful 설계 원칙 복습
    - 엔드포인트 네이밍
    - HTTP 메서드 선택
  - Basic (15min):
    - 좋은 설계 vs 나쁜 설계
    - 실제 서비스 API 분석 시작

### 2교시: REST API 설계 + 버전 관리 ⭐⭐⭐

- **REST 설계 실습 (30min)**:
  - Basic 완성 (15min):
    - 실제 서비스 API 분석
    - 네이밍 패턴
  - Practice (12min):
    - 도서관 시스템 API 설계
  - Exercise (3min):
    - 쇼핑몰 API 설계

- **API 버전 관리 (20min)**:
  - 개념 (5min):
    - 왜 필요한가?
    - 하위 호환성
    - 버전 관리 전략
  - Basic (10min):

    ```python
    from fastapi import APIRouter

    # v1
    router_v1 = APIRouter(prefix="/api/v1", tags=["v1"])

    @router_v1.get("/users")
    def get_users_v1():
        return {"version": "v1", "users": [...]}

    # v2 (개선된 응답 구조)
    router_v2 = APIRouter(prefix="/api/v2", tags=["v2"])

    @router_v2.get("/users")
    def get_users_v2():
        return {
            "version": "v2",
            "data": [...],
            "meta": {"total": 10, "page": 1}
        }

    # 앱에 등록
    app.include_router(router_v1)
    app.include_router(router_v2)
    ```

  - Practice (3min): 버전별 API 작성
  - Exercise (2min): v1 → v2 마이그레이션 설계

> **중요 추가**: 프로덕션에서 필수인 API 버전 관리!

### 3교시: requests 기초 + 라우터 분리 ⭐⭐ (수정!)

- **requests 기초 (25min)**: ← Day 7에서 이동!
  - 개념 (5min): Python으로 HTTP 요청, 외부 API 호출
  - Basic (15min):

    ```python
    import requests

    # GET 요청
    response = requests.get("https://api.github.com/users/octocat")
    data = response.json()  # 자동 JSON 파싱!
    print(data["name"])

    # POST 요청
    response = requests.post(
        "https://jsonplaceholder.typicode.com/posts",
        json={"title": "foo", "body": "bar", "userId": 1}
    )
    print(response.status_code)  # 201

    # 상태 코드 확인
    if response.status_code == 200:
        print("성공!")
    ```

  - Practice (3min): 공개 API 호출 (JSONPlaceholder)
  - Exercise (2min): GitHub API로 사용자 정보 가져오기

- **라우터 분리 (25min)**:
  - 개념 (5min):
    - APIRouter
    - 코드 구조화
    - 관심사 분리
  - Basic (12min):
    - APIRouter 사용
    - prefix 설정
    - tags
    - include_router
  - Practice (5min): users, posts 라우터 분리
  - Exercise (3min): 3개 이상 라우터 구성

> **중요 변경**: requests를 Day 7에서 Day 10으로 이동!
> → REST 설계 직후라 자연스럽고, 프로젝트에 바로 활용 가능!

### 4교시: 에러 처리 고도화 ⭐⭐

- **개념 (8min)**:
  - HTTPException 심화
  - 커스텀 에러
  - 일관된 에러 응답
- **Basic (20min)**:
  - 404 Not Found
  - 400 Bad Request
  - 상세 에러 메시지
  - detail 활용
- **Practice (12min)**:
  - 에러 핸들링 함수
- **Exercise (10min)**:
  - 모든 API에 에러 처리

### 5교시: 페이지네이션 + 프로젝트 준비 ⭐⭐

- **페이지네이션 (30min)**:
  - 개념 (7min): 필요성, skip/limit 패턴
  - Basic (15min):
    - skip, limit 받기
    - SQL LIMIT/OFFSET
    - 전체 개수 반환
  - Practice (8min): 페이지네이션 구현
- **프로젝트 주제 선정 (20min)**:
  - 주제 소개 (TODO, 블로그, 쇼핑몰, 게시판)
  - 팀/개인 결정
  - 주제 확정

### 6교시: 프로젝트 마무리 ⭐⭐⭐

- **요구사항 정의 (20min)**:
  - 기능 목록 작성
  - 우선순위 결정 (MVP)
  - 필수 vs 선택 기능
- **API 스펙 작성 (20min)**:
  - 엔드포인트 설계
  - Request/Response 모델
  - HTTP 메서드 매핑
- **DB 스키마 설계 (10min)**:
  - 테이블 구조
  - 필드 정의

> **중요 변경**: 프로젝트 설계에만 집중! 구현은 7교시부터!

### 7교시: 프로젝트 구현 (1) ⭐⭐⭐

- **초기 설정 (15min)**:
  - 디렉터리 구조
  - DB 초기화
  - Pydantic 모델 작성
- **핵심 CRUD (35min)**:
  - 핵심 엔드포인트 구현
  - DB 연동
  - 기본 검증

> **중요**: 7교시부터 본격 구현! 설계와 분리!

### 8교시: 프로젝트 구현 (2) + 발표 ⭐⭐⭐

- **기능 완성 (30min)**:
  - 추가 엔드포인트
  - 에러 처리
  - 검증 강화
  - Postman 테스트
  - 코드 정리

- **간단한 발표 (20min)**:
  - 3-4팀 간단한 시연 (각 5-6min)
  - 주요 기능 소개
  - 배운 점 공유
  - 질의응답

> **중요 변경**: 발표 시간 유지, 구현 시간 확대!
> → 완성도 UP!

---

## 📌 핵심 학습 목표 (FastAPI 중심)

### 최우선 항목 ⭐⭐⭐

1. **JSON + with문**: 딕셔너리 ↔ 텍스트, 파일 안전 처리
2. **Pydantic 모델**: Request/Response 구조화
3. **Pydantic Validator**: 커스텀 검증
4. **경로/쿼리 매개변수**: API 엔드포인트 설계
5. **CRUD 작업**: 데이터베이스 연동
6. **SQL JOIN**: 관계형 DB 이해
7. **REST API 설계**: RESTful 원칙 적용
8. **API 버전 관리**: v1, v2 설계
9. **에러 처리**: HTTPException, 상태 코드
10. **requests**: 외부 API 호출
11. **Postman**: API 테스팅

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

## 📝 v10.0 주요 변경사항

1. ✅ **Day 6-1교시**: 환경 구축 제거 → JSON/with문에 집중
2. ✅ **Day 7-1교시**: 환경 구축 추가 (30분) → 바로 FastAPI 시작
3. ✅ **Day 7-2교시**: requests 제거 → FastAPI + 문서화에 집중
4. ✅ **Day 10-3교시**: requests 추가 + 라우터 분리
5. ✅ v9.0 모든 개선사항 유지

**핵심 개선:**

- 설치하자마자 바로 사용!
- requests를 적절한 시기에 배움
- 프로젝트에 바로 활용 가능

---

## 🎯 학습 후 다음 단계

### 심화 과정 (Day 11-15)

- 프로젝트 구조와 의존성 주입
- 인증 (JWT, OAuth2)
- 권한 관리
- 로깅, 테스팅 (프로덕션 필수!)
- 최종 프로젝트

---
