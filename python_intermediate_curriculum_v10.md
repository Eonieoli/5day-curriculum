# Python 응용 과정 커리큘럼 v10

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

- 복습 퀴즈: 10분
- 핵심 복습: 15분
- 새 내용: 25분

---

## Day 6: 웹과 API의 이해

### 1교시: 복습 + JSON/with문 시작 ⭐⭐⭐

- **복습 퀴즈 (10분)**: Python 기초 핵심 (딕셔너리, 타입 힌트, 함수)
- **핵심 복습 (10분)**:
  - 딕셔너리 복습 (JSON의 기초)
  - 타입 힌트 복습
  - 간단한 Q&A
- **JSON + with문 시작 (30분)**:
  - 개념 (10분):
    - with문이란? 자동 close
    - JSON이란? 딕셔너리 ↔ 텍스트
    - 웹에서 데이터 주고받기
    - FastAPI에서의 역할
  - Basic (20분):
    - with open() 기본: `with open('file.json', 'r') as f:`
    - JSON 메모리 변환 시작: `json.dumps()`, `json.loads()`

### 2교시: JSON 기초 + with문 ⭐⭐⭐

- **Basic 완성 (22분)**:
  - JSON 메모리 변환 완성 (8분):
    ```python
    import json

    user = {"name": "Alice", "age": 25}

    # 딕셔너리 → JSON 문자열
    json_str = json.dumps(user, indent=2)

    # JSON 문자열 → 딕셔너리
    user_dict = json.loads(json_str)
    ```

  - JSON 파일 입출력 (14분):
    ```python
    # 저장
    with open('user.json', 'w') as f:
        json.dump(user, f, indent=2)

    # 로드
    with open('user.json', 'r') as f:
        user = json.load(f)

    # 실전 예제: 설정 파일, 데이터 저장
    ```
- **Practice (18분)**:
  - 학생 정보 딕셔너리 → JSON 파일 저장
  - JSON 파일 읽기 → 딕셔너리로 변환
  - 데이터 수정 → 다시 JSON 저장
- **Exercise (10분)**:
  - 상품 목록 JSON 관리
    - 상품 추가
    - 목록 조회
    - 가격 수정

### 3교시: 웹의 동작 원리 ⭐⭐

- **개념 (10분)**:
  - 클라이언트-서버 모델
  - 브라우저 역할
  - URL 구조

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

- **개념 (5분)**:
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

### 1교시: Day 6 복습 + 환경 구축 + FastAPI 시작 ⭐⭐⭐

- **복습 퀴즈 (5분)**: JSON, HTTP, REST
- **환경 구축 (30분)**:
  - 가상환경 생성 (10분):
    - `python -m venv venv`
    - 개념 설명: 왜 가상환경이 필요한가?
  - 활성화 (5분):
    - Windows: `venv\Scripts\activate`
    - Git Bash: `source venv/Scripts/activate`
    - Mac/Linux: `source venv/bin/activate`
  - FastAPI 설치 (10분):
    - `pip install fastapi uvicorn`
    - 설치 확인 (`pip list`)
    - 버전 확인
  - 테스트 (5분):
    - `import fastapi` 테스트
    - 간단한 코드 실행
- **FastAPI 소개 (15분)**:
  - FastAPI란?
  - 특징과 장점
  - 다른 프레임워크 비교
  - Hello World 준비

### 2교시: FastAPI 첫 API + 자동 문서화 ⭐⭐⭐

- **FastAPI 첫 API (30분)**:
  - Basic (20분):
    - Hello World API 완성
    - uvicorn 실행
    - 브라우저 확인
    - --reload 옵션
    - 여러 엔드포인트 추가
  - Practice (10분):
    - 함께 첫 API 만들기
    - 자기소개 API
    - 간단한 계산 API

- **자동 문서화 (20분)**:
  - 개념 (5분):
    - Swagger UI
    - ReDoc
    - 자동 문서화 장점
  - Basic (10분):
    - /docs 접속
    - /redoc 접속
    - 문서에서 API 테스트
    - docstring 추가
  - Practice (5분):
    - 여러 API 만들고 문서 확인

### 3교시: 자동 문서화 심화 ⭐⭐⭐

- **Basic (20분)**:
  - 설명 추가
  - 태그 추가
  - 문서 커스터마이징
  - 실전 예제
- **Practice (20분)**:
  - 여러 API 만들고 문서 확인
  - 설명 추가
  - 태그로 그룹화
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

- **개념 (8분)**:
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
- **Exercise (12분)**:
  - 복합 API 만들기

### 7교시: 종합 실습 - 경로+쿼리 조합 ⭐⭐

- **개념 (5분)**: 실전 API 패턴 복습
- **Basic (15분)**:
  - 복합 엔드포인트 설계
  - 실전 예제 (사용자의 게시글)
  - Postman 테스트 전략
- **Practice (20분)**:
  - 상품 검색 API (카테고리+가격+정렬)
  - 사용자 프로필 + 활동 내역
  - 페이지네이션 기본 (skip/limit)
- **Exercise (10분)**:
  - 복잡한 검색 API
  - 여러 필터 조합

### 8교시: Day 7 종합 실습

- **복습 퀴즈 (10분)**: FastAPI 기본, 경로/쿼리 매개변수
- **🟢 기초 Problem (15분)**: 간단한 도서관 API (책 조회)
- **🟡 응용 Problem (15분)**: 쇼핑몰 상품 API (경로+쿼리)
- **🔴 도전 Problem (10분)**: 복잡한 필터링 API

---

## Day 8: Pydantic과 Request/Response

### 1교시: Day 7 복습 + Pydantic 시작

- **복습 퀴즈 (10분)**: FastAPI 기본, 매개변수
- **핵심 복습 (15분)**:
  - 경로/쿼리 매개변수 복습
  - 자동 문서 확인
  - 간단한 Q&A
- **Pydantic 기초 시작 (25분)**:
  - 개념 (10분):
    - Pydantic이란?
    - BaseModel
    - 자동 검증
    - FastAPI에서의 역할
  - Basic (15분):
    - BaseModel 상속
    - 필드 정의
    - 인스턴스 생성

### 2교시: Pydantic + Request/Response 통합 ⭐⭐⭐

- **Pydantic 기초 완성 (15분)**:
  - Basic (7분): 자동 타입 변환 예제
  - Practice (5분): User, Product 모델
  - Exercise (3분): Post, Comment 모델

- **Request Body (15분)**:
  - 개념 (3분): POST/PUT, JSON 매핑
  - Basic (8분):
    - POST 엔드포인트
    - Pydantic 모델로 받기
    - 자동 검증
    - 에러 응답 (422)
  - Practice (4분): 사용자 생성 API

- **Response Model (15분)**:
  - 개념 (3분): response_model, 민감정보 제외
  - Basic (8분):
    - response_model 지정
    - 비밀번호 제외 패턴
    - List[Model] 반환
  - Practice (4분): 안전한 응답

- **통합 예제 (5분)**:
  - 회원가입 API (Request + Response)

### 3교시: Request Body 심화 ⭐⭐⭐

- **개념 (8분)**:
  - 복잡한 Request Body
  - 여러 모델 조합
  - 실전 패턴
- **Basic (22분)**:
  - 중첩 모델
  - 리스트 필드
  - 선택적 필드
  - 실전 예제
- **Practice (12분)**:
  - 상품 등록 API (복잡한 구조)
  - 주문 API (여러 상품)
- **Exercise (8분)**:
  - 게시글 작성 API (태그, 카테고리 포함)

### 4교시: Pydantic 검증 + Validator ⭐⭐⭐

- **Field 검증 (30분)**:
  - 개념 (7분):
    - Field() 함수
    - 검증 규칙
    - 에러 메시지
    - 보안
  - Basic (15분):
    - 최소/최대값
    - 길이 제한
    - 정규식
    - 기본값
  - Practice (5분): 회원가입 모델 (이메일, 비밀번호)
  - Exercise (3분): 상품 등록 검증

- **Pydantic Validator (20분)**:
  - 개념 (5분): 커스텀 검증의 필요성
  - Basic (10분):
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
  - Practice (3분): 복잡한 검증 규칙
  - Exercise (2분): 커스텀 validator 작성

### 5교시: Response Model 심화 ⭐⭐

- **개념 (8분)**:
  - response_model 심화
  - 응답 데이터 제어
  - 성능 최적화
- **Basic (20분)**:
  - 선택적 필드 제거
  - response_model_exclude
  - response_model_include
  - List[Model] 심화
- **Practice (12분)**:
  - 사용자 목록 (비밀번호 제외)
  - 상품 목록 (재고 제외)
- **Exercise (10분)**:
  - 안전한 응답 모델 설계

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
- **Exercise (10분)**:
  - 유연한 업데이트 API

### 8교시: Day 8 종합 실습

- **복습 퀴즈 (10분)**: Pydantic, Request/Response, Validator
- **🟢 기초 Problem (15분)**: TODO API (CRUD 기본 + 검증)
- **🟡 응용 Problem (15분)**: 블로그 API (Validator 포함)
- **🔴 도전 Problem (10분)**: 복잡한 검증 규칙

---

## Day 9: 데이터베이스 연동

### 1교시: Day 8 복습 + DB 기초 시작

- **복습 퀴즈 (10분)**: Pydantic 전체, Validator
- **핵심 복습 (15분)**:
  - Request Body 복습
  - Validator 복습
  - 간단한 Q&A
- **DB 기초 시작 (25분)**:
  - 개념 (15분):
    - 데이터베이스란?
    - RDBMS
    - SQLite 특징
    - 테이블/행/열
  - Basic (10분):
    - SQL 기본 개념
    - SQLite 브라우저 소개

### 2교시: 데이터베이스 기초 + SQLite ⭐⭐

- **SQL 기본 (30분)**:
  - Basic (22분):
    - SELECT, INSERT, UPDATE, DELETE
    - WHERE 조건
    - 간단한 예제
  - Practice (8분): SQL 문법 연습
- **SQLite 브라우저 (20분)**:
  - 설치 확인
  - 테이블 생성 실습
  - 데이터 입력/조회

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
- **Practice (10분)**:
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
- **Exercise (10분)**:
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
- **Practice (13분)**:
  - 업데이트 함수
  - 삭제 함수
- **Exercise (10분)**:
  - 수정/삭제 API

### 7교시: FastAPI + SQLite 통합 + JOIN 기초 ⭐⭐⭐

- **FastAPI + SQLite 통합 (25분)**:
  - 개념 (5분): 엔드포인트에서 DB 작업
  - Basic (12분):
    - CRUD API 전체 구현
    - Pydantic + DB 조합
  - Practice (5분): 간단한 게시판 API
  - Exercise (3분): TODO API에 DB 적용

- **SQL JOIN 기초 (25분)**:
  - 개념 (8분):
    - 왜 필요한가? (단일 테이블의 한계)
    - 1:N 관계 (users - posts)
    - Foreign Key 개념
  - Basic (12분):
    ```sql
    -- users 테이블
    CREATE TABLE users (
        id INTEGER PRIMARY KEY,
        name TEXT,
        email TEXT
    );

    -- posts 테이블 (user_id가 Foreign Key)
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
  - Practice (3분):
    - 사용자-게시글 JOIN 쿼리
  - Exercise (2분):
    - 댓글-작성자 JOIN

### 8교시: Day 9 종합 실습

- **복습 퀴즈 (10분)**: SQL, SQLite, CRUD, JOIN
- **🟢 기초 Problem (15분)**: 간단한 메모 API (DB 포함)
- **🟡 응용 Problem (15분)**: 사용자 관리 시스템 (관계 포함)
- **🔴 도전 Problem (10분)**: JOIN을 활용한 복합 조회

---

## Day 10: REST API 설계 및 프로젝트

### 1교시: Day 9 복습 + REST 설계 시작

- **복습 퀴즈 (10분)**: 데이터베이스, CRUD, JOIN
- **핵심 복습 (15분)**:
  - FastAPI + DB 통합 복습
  - SQL JOIN 복습
  - 간단한 Q&A
- **REST 설계 시작 (25분)**:
  - 개념 (10분):
    - RESTful 설계 원칙 복습
    - 엔드포인트 네이밍
    - HTTP 메서드 선택
  - Basic (15분):
    - 좋은 설계 vs 나쁜 설계
    - 실제 서비스 API 분석 시작

### 2교시: REST API 설계 + 버전 관리 ⭐⭐⭐

- **REST 설계 실습 (30분)**:
  - Basic 완성 (15분):
    - 실제 서비스 API 분석
    - 네이밍 패턴
  - Practice (12분):
    - 도서관 시스템 API 설계
  - Exercise (3분):
    - 쇼핑몰 API 설계

- **API 버전 관리 (20분)**:
  - 개념 (5분):
    - 왜 필요한가?
    - 하위 호환성
    - 버전 관리 전략
  - Basic (10분):
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
  - Practice (3분): 버전별 API 작성
  - Exercise (2분): v1 → v2 마이그레이션 설계

### 3교시: requests 기초 + 라우터 분리 ⭐⭐

- **requests 기초 (25분)**:
  - 개념 (5분): Python으로 HTTP 요청, 외부 API 호출
  - Basic (15분):
    ```python
    import requests

    # GET 요청
    response = requests.get("https://api.github.com/users/octocat")
    data = response.json()  # 자동 JSON 파싱
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
  - Practice (3분): 공개 API 호출 (JSONPlaceholder)
  - Exercise (2분): GitHub API로 사용자 정보 가져오기

- **라우터 분리 (25분)**:
  - 개념 (5분):
    - APIRouter
    - 코드 구조화
    - 관심사 분리
  - Basic (12분):
    - APIRouter 사용
    - prefix 설정
    - tags
    - include_router
  - Practice (5분): users, posts 라우터 분리
  - Exercise (3분): 3개 이상 라우터 구성

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
  - 개념 (7분): 필요성, skip/limit 패턴
  - Basic (15분):
    - skip, limit 받기
    - SQL LIMIT/OFFSET
    - 전체 개수 반환
  - Practice (8분): 페이지네이션 구현
- **프로젝트 주제 선정 (20분)**:
  - 주제 소개 (TODO, 블로그, 쇼핑몰, 게시판)
  - 팀/개인 결정
  - 주제 확정

### 6교시: 프로젝트 마무리 ⭐⭐⭐

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

- **기능 완성 (30분)**:
  - 추가 엔드포인트
  - 에러 처리
  - 검증 강화
  - Postman 테스트
  - 코드 정리

- **간단한 발표 (20분)**:
  - 3-4팀 간단한 시연 (각 5-6분)
  - 주요 기능 소개
  - 배운 점 공유
  - 질의응답

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

## 🎯 학습 후 다음 단계

### 심화 과정 (Day 11-15)

- 프로젝트 구조와 의존성 주입
- 인증 (JWT, OAuth2)
- 권한 관리
- 로깅, 테스팅
- 최종 프로젝트

---
