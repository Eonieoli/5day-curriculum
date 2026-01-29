# Python 응용 과정 커리큘럼 v10.0 (SQLAlchemy 버전)

> **📌 이 버전에 대하여**
> 
> 이 문서는 **SQLAlchemy를 사용하는 버전**입니다.
> - 회사 교육용: `python_intermediate_curriculum_v10.md` (raw SQL 버전)
> - 개인 공부용: 이 문서 (SQLAlchemy 버전)
> 
> **Day 9에서 SQLAlchemy를 완전히 배웁니다!**
> - SQLAlchemy 기초부터 관계(relationship)까지
> - Day 10 프로젝트에서 SQLAlchemy 활용

## 📋 과정 개요

- **과정명**: Python 응용 과정 (SQLAlchemy 버전)
- **목표**: 웹 개념 이해 및 FastAPI + SQLAlchemy로 REST API 개발
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

> **참고**: Day 6은 raw SQL 버전과 동일합니다.

### 1교시: 복습 + JSON/with문 시작 ⭐⭐⭐

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

> **참고**: Day 7은 raw SQL 버전과 동일합니다.

### 1교시: Day 6 복습 + 환경 구축 + FastAPI 시작 ⭐⭐⭐

- **복습 퀴즈 (5min)**: JSON, HTTP, REST (짧게!)
- **환경 구축 (30min)**:
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

### 2교시: FastAPI 첫 API + 자동 문서화 ⭐⭐⭐

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

### 8교시: Day 7 종합 실습

- **복습 퀴즈 (10min)**: FastAPI 기본, 경로/쿼리 매개변수
- **🟢 기초 Problem (15min)**: 간단한 도서관 API (책 조회)
- **🟡 응용 Problem (15min)**: 쇼핑몰 상품 API (경로+쿼리)
- **🔴 도전 Problem (10min)**: 복잡한 필터링 API

---

## Day 8: Pydantic과 Request/Response

> **참고**: Day 8은 raw SQL 버전과 동일합니다.

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

## Day 9: SQLAlchemy 완전 정복 ⭐⭐⭐

> **주요 변경**: 이 Day가 raw SQL 버전과 가장 다릅니다!

### 1교시: Day 8 복습 + DB 기초 + Python 연동 시작

- **복습 퀴즈 (10min)**: Pydantic 전체, Validator
- **핵심 복습 (10min)**: 
  - Request Body 복습
  - Validator 복습
  - 간단한 Q&A

- **DB 기초 + Python 연동 시작 (30min)**:
  - **DB 기초 개념 (15min)**:
    - 데이터베이스란?
    - RDBMS
    - SQLite 특징
    - 테이블/행/열
    - SQL이란? (간단히)
  
  - **Python DB 연동 기초 (15min)**:
    ```python
    # sqlite3 모듈 간단히 맛보기
    import sqlite3
    
    # 연결
    conn = sqlite3.connect("app.db")
    cursor = conn.cursor()
    
    # 테이블 생성
    cursor.execute("""
        CREATE TABLE IF NOT EXISTS users (
            id INTEGER PRIMARY KEY,
            email TEXT,
            name TEXT
        )
    """)
    
    # 데이터 삽입 (파라미터 바인딩 중요!)
    cursor.execute(
        "INSERT INTO users (email, name) VALUES (?, ?)",
        ("alice@example.com", "Alice")
    )
    
    # 커밋 & 종료
    conn.commit()
    conn.close()
    ```
    - 파라미터 바인딩 (?, ?)
    - SQL Injection 방지
    - commit의 중요성

### 2교시: FastAPI + raw SQL 빠른 통합 ⭐⭐

- **개념 (8min)**:
  - FastAPI에서 DB 사용
  - CRUD 패턴
  - 간단한 통합

- **Basic (25min)**:
  ```python
  from fastapi import FastAPI, HTTPException
  import sqlite3
  from pydantic import BaseModel
  
  app = FastAPI()
  
  class User(BaseModel):
      email: str
      name: str
  
  class UserResponse(BaseModel):
      id: int
      email: str
      name: str
  
  def get_db():
      conn = sqlite3.connect("app.db")
      conn.row_factory = sqlite3.Row  # 딕셔너리처럼 사용
      return conn
  
  @app.post("/users", response_model=UserResponse)
  def create_user(user: User):
      conn = get_db()
      cursor = conn.cursor()
      cursor.execute(
          "INSERT INTO users (email, name) VALUES (?, ?)",
          (user.email, user.name)
      )
      conn.commit()
      user_id = cursor.lastrowid
      conn.close()
      
      return {"id": user_id, "email": user.email, "name": user.name}
  
  @app.get("/users/{user_id}", response_model=UserResponse)
  def get_user(user_id: int):
      conn = get_db()
      cursor = conn.cursor()
      cursor.execute("SELECT * FROM users WHERE id = ?", (user_id,))
      user = cursor.fetchone()
      conn.close()
      
      if not user:
          raise HTTPException(status_code=404, detail="User not found")
      
      return dict(user)
  ```

- **Practice (12min)**:
  - 간단한 CRUD API 만들기
  - Postman 테스트

- **Exercise (5min)**:
  - TODO API 만들기 (raw SQL)

> **중요**: 이제 raw SQL의 문제점을 체감했으니 SQLAlchemy로!

### 3교시: SQLAlchemy 개념 + 환경 설정 ⭐⭐⭐

- **개념 (10min)**:
  - **ORM이란?**
    - Object-Relational Mapping
    - Python 클래스 ↔ DB 테이블
  - **raw SQL vs ORM**:
    ```python
    # raw SQL
    cursor.execute("SELECT * FROM users WHERE id = ?", (user_id,))
    user = cursor.fetchone()
    
    # SQLAlchemy ORM
    user = db.query(User).filter(User.id == user_id).first()
    ```
  - **왜 SQLAlchemy?**
    - 타입 안정성
    - 자동완성
    - 관계 관리 쉬움
    - 코드 재사용성

- **설치 (5min)**:
  ```bash
  pip install sqlalchemy
  ```

- **기본 구조 (15min)**:
  ```python
  # database.py
  from sqlalchemy import create_engine
  from sqlalchemy.ext.declarative import declarative_base
  from sqlalchemy.orm import sessionmaker
  
  # 데이터베이스 URL
  SQLALCHEMY_DATABASE_URL = "sqlite:///./app.db"
  
  # Engine 생성
  engine = create_engine(
      SQLALCHEMY_DATABASE_URL,
      connect_args={"check_same_thread": False}  # SQLite only
  )
  
  # Session 클래스
  SessionLocal = sessionmaker(
      autocommit=False,
      autoflush=False,
      bind=engine
  )
  
  # Base 클래스 (모든 모델의 부모)
  Base = declarative_base()
  ```
  - **Engine**: DB 연결 관리
  - **Session**: DB 작업 수행
  - **Base**: 모델 정의의 기초

- **첫 모델 (20min)**:
  ```python
  # models.py
  from sqlalchemy import Column, Integer, String
  from database import Base
  
  class User(Base):
      __tablename__ = "users"  # 테이블 이름
      
      id = Column(Integer, primary_key=True, index=True)
      email = Column(String, unique=True, index=True)
      name = Column(String)
  
  # 테이블 생성
  # main.py
  from database import engine
  from models import Base
  
  Base.metadata.create_all(bind=engine)
  ```

### 4교시: SQLAlchemy 모델 정의 ⭐⭐⭐

- **개념 (8min)**:
  - Column 타입
  - 제약조건
  - 인덱스

- **Basic (24min)**:
  ```python
  from sqlalchemy import Column, Integer, String, Float, DateTime, Boolean, Text
  from datetime import datetime
  from database import Base
  
  class Product(Base):
      __tablename__ = "products"
      
      # Column 타입들
      id = Column(Integer, primary_key=True, index=True)
      name = Column(String(100), nullable=False)  # 길이 제한, NOT NULL
      description = Column(Text)  # 긴 텍스트
      price = Column(Float, nullable=False)
      stock = Column(Integer, default=0)  # 기본값
      is_active = Column(Boolean, default=True)
      created_at = Column(DateTime, default=datetime.utcnow)
      
      # 제약조건
      # unique=True: 중복 불가
      # index=True: 인덱스 생성 (검색 빠름)
      # nullable=False: NULL 불가
      # default: 기본값
  
  class Post(Base):
      __tablename__ = "posts"
      
      id = Column(Integer, primary_key=True, index=True)
      title = Column(String(200), nullable=False, index=True)
      content = Column(Text, nullable=False)
      published = Column(Boolean, default=False)
      created_at = Column(DateTime, default=datetime.utcnow)
      updated_at = Column(DateTime, default=datetime.utcnow, onupdate=datetime.utcnow)
  ```

- **Practice (13min)**:
  - Product 모델 작성
  - Post 모델 작성
  - 테이블 생성 확인

- **Exercise (5min)**:
  - Comment 모델 작성
  - Category 모델 작성

### 5교시: SQLAlchemy 세션 + Create ⭐⭐⭐

- **세션 관리 (12min)**:
  ```python
  from sqlalchemy.orm import Session
  from database import SessionLocal
  
  # 세션 생성
  db = SessionLocal()
  
  try:
      # DB 작업
      pass
  finally:
      db.close()  # 항상 닫기!
  
  # FastAPI 의존성 패턴 (중요!)
  def get_db():
      db = SessionLocal()
      try:
          yield db
      finally:
          db.close()
  
  # 엔드포인트에서 사용
  from fastapi import Depends
  
  @app.get("/users")
  def get_users(db: Session = Depends(get_db)):
      users = db.query(User).all()
      return users
  ```

- **Create 작업 (20min)**:
  ```python
  from sqlalchemy.orm import Session
  from models import User
  from schemas import UserCreate
  
  def create_user(db: Session, user: UserCreate):
      # 1. 모델 인스턴스 생성
      db_user = User(
          email=user.email,
          name=user.name
      )
      
      # 2. 세션에 추가
      db.add(db_user)
      
      # 3. 커밋 (DB에 실제 저장)
      db.commit()
      
      # 4. 새로고침 (ID 등 DB에서 생성된 값 가져옴)
      db.refresh(db_user)
      
      return db_user
  
  # FastAPI 엔드포인트
  @app.post("/users", response_model=UserResponse)
  def create_user_endpoint(
      user: UserCreate,
      db: Session = Depends(get_db)
  ):
      return create_user(db, user)
  ```

- **Practice (10min)**:
  - 사용자 생성 함수
  - 상품 생성 함수

- **Exercise (8min)**:
  - 게시글 생성 API

### 6교시: SQLAlchemy Read (조회) ⭐⭐⭐

- **개념 (7min)**:
  - query() 메서드
  - filter() vs filter_by()
  - 조회 메서드들

- **Basic (23min)**:
  ```python
  from sqlalchemy.orm import Session
  from models import User, Post
  
  # 전체 조회
  def get_all_users(db: Session):
      return db.query(User).all()
  
  # 단일 조회 (ID로)
  def get_user(db: Session, user_id: int):
      return db.query(User).filter(User.id == user_id).first()
  
  # 조건 조회 (filter)
  def get_user_by_email(db: Session, email: str):
      return db.query(User).filter(User.email == email).first()
  
  # 조건 조회 (filter_by) - 간단할 때
  def get_user_by_email_v2(db: Session, email: str):
      return db.query(User).filter_by(email=email).first()
  
  # 여러 조건
  def search_posts(db: Session, keyword: str, published: bool = True):
      return db.query(Post).filter(
          Post.title.contains(keyword),
          Post.published == published
      ).all()
  
  # 정렬
  def get_posts_sorted(db: Session):
      return db.query(Post).order_by(Post.created_at.desc()).all()
  
  # 제한
  def get_recent_posts(db: Session, limit: int = 10):
      return db.query(Post).order_by(
          Post.created_at.desc()
      ).limit(limit).all()
  
  # 페이지네이션
  def get_posts_paginated(db: Session, skip: int = 0, limit: int = 10):
      return db.query(Post).offset(skip).limit(limit).all()
  
  # 개수
  def count_users(db: Session):
      return db.query(User).count()
  ```

- **Practice (12min)**:
  - 다양한 조회 함수 작성
  - 검색 API
  - 페이지네이션 API

- **Exercise (8min)**:
  - 복잡한 조건 조회
  - 정렬 + 필터링

### 7교시: SQLAlchemy Update + Delete + 관계 ⭐⭐⭐

- **Update & Delete (25min)**:
  ```python
  # Update
  def update_user(db: Session, user_id: int, email: str = None, name: str = None):
      user = db.query(User).filter(User.id == user_id).first()
      if not user:
          return None
      
      # 값 수정
      if email:
          user.email = email
      if name:
          user.name = name
      
      db.commit()
      db.refresh(user)
      return user
  
  # Delete
  def delete_user(db: Session, user_id: int):
      user = db.query(User).filter(User.id == user_id).first()
      if not user:
          return False
      
      db.delete(user)
      db.commit()
      return True
  ```

- **관계 (relationship) (25min)**:
  ```python
  from sqlalchemy import Column, Integer, String, ForeignKey
  from sqlalchemy.orm import relationship
  from database import Base
  
  class User(Base):
      __tablename__ = "users"
      
      id = Column(Integer, primary_key=True, index=True)
      email = Column(String, unique=True, index=True)
      name = Column(String)
      
      # 관계 정의 (1:N - User : Posts)
      posts = relationship("Post", back_populates="user")
  
  class Post(Base):
      __tablename__ = "posts"
      
      id = Column(Integer, primary_key=True, index=True)
      title = Column(String)
      content = Column(String)
      
      # Foreign Key
      user_id = Column(Integer, ForeignKey("users.id"))
      
      # 관계 정의 (N:1 - Post : User)
      user = relationship("User", back_populates="posts")
  
  # 사용 예시
  def create_post_for_user(db: Session, user_id: int, title: str, content: str):
      post = Post(
          title=title,
          content=content,
          user_id=user_id  # Foreign Key 설정
      )
      db.add(post)
      db.commit()
      db.refresh(post)
      return post
  
  def get_user_with_posts(db: Session, user_id: int):
      user = db.query(User).filter(User.id == user_id).first()
      # user.posts로 자동으로 게시글 접근!
      return user
  
  # FastAPI 엔드포인트
  @app.get("/users/{user_id}/posts")
  def get_user_posts(user_id: int, db: Session = Depends(get_db)):
      user = db.query(User).filter(User.id == user_id).first()
      if not user:
          raise HTTPException(status_code=404, detail="User not found")
      return user.posts  # relationship 덕분에 자동으로!
  ```

### 8교시: FastAPI + SQLAlchemy 통합 종합 실습 ⭐⭐⭐

- **복습 퀴즈 (10min)**: SQLAlchemy 전체 (모델, Session, CRUD, relationship)

- **🟢 기초 Problem (15min)**: 간단한 메모 API (SQLAlchemy)
  - 메모 생성, 조회, 수정, 삭제
  - Pydantic 스키마 + SQLAlchemy 모델

- **🟡 응용 Problem (15min)**: 사용자-게시글 관계 API
  - User 모델 + Post 모델
  - relationship 활용
  - 사용자의 게시글 조회

- **🔴 도전 Problem (10min)**: 복잡한 관계 + 조회
  - User - Post - Comment (3단계 관계)
  - 특정 사용자의 댓글 단 게시글 조회

---

## Day 10: REST API 설계 및 프로젝트 (SQLAlchemy)

### 1교시: Day 9 복습 + REST 설계 시작

- **복습 퀴즈 (10min)**: SQLAlchemy, CRUD, relationship
- **핵심 복습 (15min)**: 
  - SQLAlchemy 모델 복습
  - relationship 복습
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

### 3교시: requests 기초 + 라우터 분리 ⭐⭐

- **requests 기초 (25min)**:
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

### 5교시: 페이지네이션 (SQLAlchemy) + 프로젝트 준비 ⭐⭐

- **페이지네이션 (30min)**:
  - 개념 (7min): 필요성, skip/limit 패턴
  - Basic (15min):
    ```python
    from sqlalchemy.orm import Session
    from fastapi import Depends
    
    @app.get("/posts")
    def get_posts(
        skip: int = 0,
        limit: int = 10,
        db: Session = Depends(get_db)
    ):
        # SQLAlchemy 페이지네이션
        posts = db.query(Post).offset(skip).limit(limit).all()
        
        # 전체 개수
        total = db.query(Post).count()
        
        return {
            "data": posts,
            "total": total,
            "skip": skip,
            "limit": limit
        }
    ```
  - Practice (8min): 페이지네이션 구현
- **프로젝트 주제 선정 (20min)**:
  - 주제 소개 (TODO, 블로그, 쇼핑몰, 게시판)
  - 팀/개인 결정
  - 주제 확정
  - **SQLAlchemy 사용 필수!**

### 6교시: 프로젝트 마무리 (SQLAlchemy) ⭐⭐⭐

- **요구사항 정의 (20min)**:
  - 기능 목록 작성
  - 우선순위 결정 (MVP)
  - 필수 vs 선택 기능
  - **SQLAlchemy 모델 설계 포함!**

- **API 스펙 작성 (20min)**:
  - 엔드포인트 설계
  - Request/Response 모델 (Pydantic)
  - HTTP 메서드 매핑

- **DB 스키마 설계 (10min)**:
  - SQLAlchemy 모델 구조
  - relationship 설계
  - Foreign Key 관계

### 7교시: 프로젝트 구현 (1) - SQLAlchemy 모델 ⭐⭐⭐

- **초기 설정 (15min)**:
  - 디렉터리 구조
  ```
  project/
  ├── app/
  │   ├── __init__.py
  │   ├── main.py
  │   ├── database.py
  │   ├── models.py      # SQLAlchemy 모델
  │   ├── schemas.py     # Pydantic 스키마
  │   └── routers/
  │       ├── __init__.py
  │       └── ...
  ├── .env
  └── requirements.txt
  ```
  - database.py 설정
  - Base 생성

- **SQLAlchemy 모델 작성 (20min)**:
  ```python
  # models.py
  from sqlalchemy import Column, Integer, String, ForeignKey, DateTime
  from sqlalchemy.orm import relationship
  from database import Base
  from datetime import datetime
  
  class User(Base):
      __tablename__ = "users"
      
      id = Column(Integer, primary_key=True, index=True)
      email = Column(String, unique=True, index=True)
      name = Column(String)
      
      # 관계
      posts = relationship("Post", back_populates="user")
  
  class Post(Base):
      __tablename__ = "posts"
      
      id = Column(Integer, primary_key=True, index=True)
      title = Column(String)
      content = Column(String)
      user_id = Column(Integer, ForeignKey("users.id"))
      created_at = Column(DateTime, default=datetime.utcnow)
      
      # 관계
      user = relationship("User", back_populates="posts")
  ```

- **핵심 CRUD (15min)**:
  ```python
  # 엔드포인트에서 SQLAlchemy 사용
  @app.post("/users")
  def create_user(user: UserCreate, db: Session = Depends(get_db)):
      db_user = User(email=user.email, name=user.name)
      db.add(db_user)
      db.commit()
      db.refresh(db_user)
      return db_user
  ```

### 8교시: 프로젝트 구현 (2) + 발표 ⭐⭐⭐

- **기능 완성 (30min)**:
  - 추가 엔드포인트 (SQLAlchemy 활용)
  - relationship 활용
  - 에러 처리
  - 검증 강화
  - Postman 테스트
  - 코드 정리

- **간단한 발표 (20min)**:
  - 3-4팀 간단한 시연 (각 5-6min)
  - SQLAlchemy 모델 구조 설명
  - 주요 기능 소개
  - 배운 점 공유
  - 질의응답

---

## 📌 핵심 학습 목표 (FastAPI + SQLAlchemy 중심)

### 최우선 항목 ⭐⭐⭐

1. **JSON + with문**: 딕셔너리 ↔ 텍스트, 파일 안전 처리
2. **Pydantic 모델**: Request/Response 구조화
3. **Pydantic Validator**: 커스텀 검증
4. **경로/쿼리 매개변수**: API 엔드포인트 설계
5. **SQLAlchemy 모델**: Column, 타입, 제약조건
6. **SQLAlchemy Session**: 세션 관리, get_db() 패턴
7. **SQLAlchemy CRUD**: query, filter, add, commit, delete
8. **SQLAlchemy relationship**: 1:N 관계, Foreign Key
9. **REST API 설계**: RESTful 원칙 적용
10. **API 버전 관리**: v1, v2 설계
11. **에러 처리**: HTTPException, 상태 코드
12. **requests**: 외부 API 호출
13. **Postman**: API 테스팅

### 중요 항목 ⭐⭐

1. HTTP 프로토콜 이해
2. 라우터 분리
3. 페이지네이션

### 기본 항목 ⭐

1. 웹 동작 원리
2. 자동 문서화

---

## 📝 SQLAlchemy 버전 주요 차이점

### raw SQL 버전 (회사 교육용)과의 차이:

#### Day 9 구조 비교:

**raw SQL 버전:**
```
1교시: 복습 + DB 기초
2교시: SQL 기본 (SELECT, INSERT, UPDATE, DELETE)
3교시: SQLite 연결
4교시: CREATE
5교시: READ
6교시: UPDATE, DELETE
7교시: FastAPI + DB 통합 + JOIN
8교시: 종합 실습
```

**SQLAlchemy 버전:**
```
1교시: 복습 + DB 기초 + Python 연동
2교시: FastAPI + raw SQL 빠른 통합 (복습 겸)
3교시: SQLAlchemy 개념 + 환경 설정
4교시: SQLAlchemy 모델 정의
5교시: SQLAlchemy Session + Create
6교시: SQLAlchemy Read
7교시: SQLAlchemy Update + Delete + 관계
8교시: FastAPI + SQLAlchemy 통합 종합 실습
```

#### 코드 비교:

```python
# raw SQL 버전
cursor.execute("SELECT * FROM users WHERE id = ?", (user_id,))
user = cursor.fetchone()

# SQLAlchemy 버전
user = db.query(User).filter(User.id == user_id).first()
```

```python
# raw SQL 버전 (관계)
cursor.execute("""
    SELECT posts.*, users.name
    FROM posts
    JOIN users ON posts.user_id = users.id
""")

# SQLAlchemy 버전 (관계)
class User(Base):
    posts = relationship("Post", back_populates="user")

user = db.query(User).filter(User.id == user_id).first()
print(user.posts)  # 자동으로 관계 데이터!
```

---

## 🎯 학습 후 다음 단계

### 심화 과정 (Day 11-15, SQLAlchemy 버전)
- 프로젝트 구조와 의존성 주입
- 인증 (JWT, OAuth2) + SQLAlchemy
- 권한 관리 + SQLAlchemy
- 로깅, 테스팅 (프로덕션 필수!)
- 최종 프로젝트 (SQLAlchemy)

### 권장 추가 학습
1. **SQLAlchemy 심화**:
   - 복잡한 쿼리 (join, group_by)
   - Alembic 마이그레이션
   - 성능 최적화

2. **비동기 SQLAlchemy** (선택):
   - async/await
   - AsyncSession

---

## 💡 버전 선택 가이드

### 회사 교육용: raw SQL 버전
- SQL 기초부터 완전히 배움
- SQL을 모르는 사람도 OK
- ORM 없이 순수 SQL 이해

### 개인 공부용: SQLAlchemy 버전 (이 문서)
- 현대적인 ORM 사용
- 타입 안정성
- 관계 관리 쉬움
- 실무에서 많이 사용

**둘 다 배우면 최고!** SQL 이해 → SQLAlchemy 활용 💪

---
