# Python 심화 과정 커리큘럼 v7.0

## 📋 과정 개요

- **과정명**: Python 심화 과정
- **목표**: 프로덕션 수준의 FastAPI 백엔드 서버 구축
- **기간**: 5일 (Day 11 ~ Day 15)
- **일일 시간**: 8교시 (명목상 50분 × 8 = 400분, 실제 약 7시간)
- **총 시간**: 약 35시간
- **선수 과정**: Python 기초 과정 (Day 1-5), Python 응용 과정 (Day 6-10)
- **휴식**: 각 교시 사이 10분, 점심 시간 1시간

## 🎯 교육 구조

### 5단계 학습 방법론

1. **개념 (Concept)**: 이론 설명, 정의, 필요성, 실무 활용
2. **Basic (Example)**: 강사가 보여주는 예제 코드 (학생은 관찰)
3. **Practice (Guided)**: 강사와 함께 타이핑하며 익히기
4. **Exercise (Independent)**: 학생이 스스로 문제 풀기
5. **Problem (Comprehensive)**: 종합 실습 (8교시, 기초/응용/도전 3단계)

### 시간 배분 원칙

**일반 교시 (1-7교시, 50분)**

- 개념: 5-15분 (복잡한 개념은 더 길게)
- Basic: 15-25분
- Practice: 10-20분
- Exercise: 10-15분

**8교시 종합 실습 (50분)**

- 복습 퀴즈: 10분
- 🟢 기초 Problem: 15분
- 🟡 응용 Problem: 15분
- 🔴 도전 Problem: 10분

**복습 교시 (매일 1교시, 50분)** ✨ NEW!

- 복습 퀴즈: 10분 (간소화!)
- 핵심 복습: 15분 (전날 가장 중요한 것만!)
- 새 내용: 25분 (바로 진도!)

**프로젝트 교시 (Day 15)**

- 구현: 1-5교시 (250분)
- 발표: 6-8교시 (150분)

---

## Day 11: 프로젝트 구조와 의존성 주입

### 1교시: 응용 과정 복습 + 프로젝트 구조 시작 ✨

- **복습 퀴즈 (10분)**: FastAPI 기본, Pydantic, CRUD, REST API
- **핵심 복습 (15분)**:
  - Pydantic 모델 복습
  - Request/Response 복습
  - 간단한 Q&A
- **프로젝트 구조 시작 (25분)**:
  - 심화 과정 소개 (5분):
    - 로드맵
    - 최종 목표 (프로덕션 레벨 API)
    - 5일 계획
  - 환경 체크 (5분):
    - 가상환경 확인
    - FastAPI 확인
  - 개념 (15분):
    - 계층 구조 (Web-Service-Data)
    - 관심사의 분리
    - 확장 가능한 구조
    - 왜 필요한가?

### 2교시: 프로젝트 구조 설계 ⭐⭐⭐

- **Basic (25분)**:
  - 디렉터리 구조
  - 파일 역할
  - **init**.py
  - 모듈 import 패턴
  - 실전 예제
- **Practice (15분)**:
  - 프로젝트 구조 만들기 (함께)
  - 파일 생성 및 조직화
- **Exercise (10분)**:
  - 자신의 프로젝트 구조 설계

### 3교시: 라우터 분리 심화 ⭐⭐

- **개념 (8분)**:
  - 도메인별 라우터
  - tags/prefix 활용
  - 계층별 책임
- **Basic (20분)**:
  - APIRouter 심화
  - include_router
  - 여러 라우터 조합
- **Practice (12분)**:
  - users, posts, comments 라우터 분리
- **Exercise (10분)**:
  - 3개 이상 도메인 라우터 구성

### 4교시: 의존성 주입 개념 ⭐⭐⭐

- **개념 (15분)**:
  - DI(Dependency Injection)란?
  - 왜 필요한가?
  - FastAPI의 Depends
  - 테스트 용이성
- **Basic (20분)**:
  - 간단한 의존성
  - 함수를 의존성으로
  - 클래스를 의존성으로
  - 의존성 체인
- **Practice (10분)**:
  - 설정 의존성
  - 로깅 의존성
- **Exercise (5분)**:
  - 커스텀 의존성 작성

### 5교시: 환경 변수 관리 ⭐⭐

- **개념 (10분)**:
  - .env 파일
  - 환경별 설정 (dev/prod)
  - 비밀 정보 관리
- **Basic (20분)**:
  - python-dotenv
  - 설정 클래스
  - Pydantic Settings
  - 환경 변수 주입
  - **환경 변수 검증** (필수 값 체크)
- **Practice (10min)**:
  - .env 파일 생성
  - Settings 클래스 작성
- **Exercise (10min)**:
  - 환경별 설정 분리

### 6교시: 데이터베이스 의존성 ⭐⭐⭐

- **개념 (12min)**:
  - get_db() 패턴
  - 연결 관리
  - 자동 close
  - yield
  - 트랜잭션
- **Basic (20min)**:
  - DB 연결 의존성
  - yield 사용
  - 에러 시 rollback
  - 실전 패턴
- **Practice (10min)**:
  - get_db() 구현
  - 엔드포인트에 적용
- **Exercise (8min)**:
  - DB 의존성 테스트

### 7교시: 계층 분리 완전 정복 ⭐⭐⭐ ✨ 통합!

- **개념 (10min)**:
  - Web(라우터) / Service(비즈니스) / Data(DB) 계층
  - 각 계층의 역할과 책임
  - 실전 프로젝트 구조

- **기본 분리 (15min)**:
  - Basic (10min):
    - 간단한 CRUD 분리
    - 함수 분리 패턴
    - 의존성 흐름
  - Practice (5min):
    - 간단한 CRUD를 계층별로 리팩토링

- **심화 분리 (15min)**: ⭐⭐⭐
  - Basic (10min):
    - 복잡한 비즈니스 로직 분리
    - Service 계층 패턴
    - 트랜잭션 관리
    - 에러 처리 계층별 전략
  - Practice (5min):
    - 게시판 API를 완전한 3계층으로

- **실습 (10min)**:
  - Exercise: 새 기능을 계층별로 구현

> **중요 통합**: Day 12-1교시 심화 내용을 여기로!
> → 하루 안에 완전 정복!

### 8교시: Day 11 종합 실습

- **복습 퀴즈 (10min)**: 프로젝트 구조, DI, 계층 분리
- **🟢 기초 Problem (15min)**: 계층 구조로 TODO API 리팩토링
- **🟡 응용 Problem (15min)**: 완전한 3계층 구조 구축 + 의존성 활용
- **🔴 도전 Problem (10min)**: 의존성 체인 최적화

---

## Day 12: 인증 기초 - 패스워드와 JWT

### 1교시: Day 11 복습 + 인증 개념 ✨ 변경!

- **복습 퀴즈 (10min)**: 프로젝트 구조, 의존성 주입, 계층 분리
- **핵심 복습 (15min)**:
  - 3계층 구조 복습
  - 의존성 주입 복습
  - 간단한 Q&A
- **인증 개념 시작 (25min)**:
  - 개념 (15min):
    - Authentication vs Authorization
    - 세션 vs 토큰
    - JWT 소개
    - 보안의 중요성
  - Basic (10min):
    - 인증 흐름 도식화
    - 토큰 기반 인증

> **중요 변경**: 계층 분리 심화 제거! Day 11-7교시로 이동!
> → 인증에 집중!

### 2교시: 인증과 인가 개념 + JWT 구조 ⭐⭐⭐

- **개념 완성 (20min)**:
  - 토큰 기반 인증 심화
  - JWT 구조 (Header/Payload/Signature)
  - 클레임(Claims)
  - 만료 시간
- **Basic (20min)**:
  - JWT 디코딩 실습 (jwt.io)
  - 페이로드 구성 예제
  - 보안 고려사항
- **Practice (10min)**:
  - JWT 분석 실습
  - 인증 시나리오 분석

### 3교시: 패스워드 해싱 ⭐⭐⭐

- **개념 (10min)**:
  - 평문 저장의 위험성
  - 해시 함수
  - Salt
- **Basic (22min)**:
  - passlib 설치 및 사용
  - 해시 생성
  - 해시 검증
  - 안전한 비교
- **Practice (10min)**:
  - 패스워드 해싱 함수 구현
- **Exercise (8min)**:
  - 해싱 도구 함수 작성

### 4교시: JWT 생성 ⭐⭐⭐

- **개념 (10min)**:
  - JWT 상세 구조
  - 클레임
  - 만료 시간
- **Basic (22min)**:
  - python-jose 설치
  - SECRET_KEY, 알고리즘
  - create_access_token() 함수
  - 페이로드 구성
- **Practice (10min)**:
  - 토큰 생성 함수 구현
- **Exercise (8min)**:
  - 커스텀 클레임 추가

### 5교시: JWT 검증 ⭐⭐⭐

- **개념 (8min)**:
  - 토큰 검증 프로세스
  - 보안 고려사항
- **Basic (22min)**:
  - verify_token() 함수
  - jwt.decode()
  - 예외 처리 (ExpiredSignatureError)
  - 서명 검증
  - 만료 확인
- **Practice (12min)**:
  - 토큰 검증 구현
  - 에러 처리 강화
- **Exercise (8min)**:
  - 토큰 검증 테스트

### 6교시: 회원가입 구현 ⭐⭐

- **개념 (7min)**:
  - 회원가입 플로우
  - 사용자 모델
  - 중복 체크
- **Basic (20min)**:
  - User 모델 (Pydantic)
  - DB 테이블
  - 중복 이메일 체크
  - 해싱 적용
- **Practice (13min)**:
  - 회원가입 API 완성
- **Exercise (10min)**:
  - 유효성 검증 강화

### 7교시: 로그인 구현 ⭐⭐⭐

- **개념 (8min)**:
  - 로그인 플로우
  - 사용자 검증
  - 토큰 발급
- **Basic (22min)**:
  - 로그인 엔드포인트
  - 이메일/패스워드 검증
  - 토큰 생성 및 반환
  - 에러 처리 (401)
- **Practice (10min)**:
  - 로그인 API 완성
- **Exercise (10min)**:
  - Postman으로 전체 흐름 테스트

### 8교시: Day 12 종합 실습

- **복습 퀴즈 (10min)**: 해싱, JWT, 인증
- **🟢 기초 Problem (15min)**: 간단한 인증 시스템 구축
- **🟡 응용 Problem (15min)**: 회원가입 + 로그인 + 토큰 검증
- **🔴 도전 Problem (10min)**: 토큰 갱신(Refresh Token) 로직

---

## Day 13: OAuth2와 권한 관리

### 1교시: Day 12 복습 + OAuth2 시작 ✨

- **복습 퀴즈 (10min)**: 패스워드 해싱, JWT, 인증
- **핵심 복습 (15min)**:
  - 로그인 재구현
  - 토큰 검증 복습
  - 간단한 Q&A
- **OAuth2 개념 시작 (25min)**:
  - 개념 (15min):
    - OAuth2란?
    - 흐름(Flow)
    - Password Flow
    - FastAPI의 OAuth2PasswordBearer
  - Basic (10min):
    - OAuth2 구조
    - tokenUrl

### 2교시: OAuth2 개념 ⭐⭐⭐

- **Basic 완성 (20min)**:
  - Bearer 토큰
  - Authorization 헤더
  - 실전 예제
- **Practice (20min)**:
  - OAuth2PasswordBearer 설정
  - 플로우 이해 확인
- **Exercise (10min)**:
  - OAuth2 패턴 적용

### 3교시: OAuth2PasswordBearer 구현 ⭐⭐⭐

- **개념 (8min)**:
  - OAuth2PasswordBearer 사용법
  - 의존성으로 활용
- **Basic (22min)**:
  - OAuth2PasswordBearer 인스턴스
  - 토큰 추출
  - 자동 문서 연동
- **Practice (12min)**:
  - 기존 인증에 OAuth2 적용
- **Exercise (8min)**:
  - 토큰 추출 테스트

### 4교시: 현재 사용자 + 전역 에러 핸들러 ⭐⭐⭐ ✨ 추가!

- **get_current_user (30min)**:
  - 개념 (7min):
    - get_current_user 패턴
    - 의존성 체인
    - 사용자 정보 활용
  - Basic (15min):
    - get_current_user() 함수
    - 토큰 검증 + DB 조회
    - HTTPException 처리
    - 의존성으로 주입
  - Practice (5min):
    - 현재 사용자 의존성 구현
  - Exercise (3min):
    - 프로필 API에 적용

- **전역 에러 핸들러 (20min)**: ✨ NEW!
  - 개념 (5min):
    - exception_handler 데코레이터
    - 일관된 에러 응답
    - 프로덕션 필수!
  - Basic (10min):
    ```python
    from fastapi import FastAPI, Request
    from fastapi.responses import JSONResponse
    
    @app.exception_handler(ValueError)
    async def value_error_handler(request: Request, exc: ValueError):
        return JSONResponse(
            status_code=400,
            content={"detail": str(exc), "type": "ValueError"}
        )
    
    @app.exception_handler(404)
    async def not_found_handler(request, exc):
        return JSONResponse(
            status_code=404,
            content={"detail": "Resource not found"}
        )
    
    # 모든 예외 처리
    @app.exception_handler(Exception)
    async def general_exception_handler(request, exc):
        logger.error(f"Unhandled error: {exc}")
        return JSONResponse(
            status_code=500,
            content={"detail": "Internal server error"}
        )
    ```
  - Practice (3min): 전역 핸들러 추가
  - Exercise (2min): 커스텀 예외 처리

> **중요 추가**: 프로덕션에서 필수인 전역 에러 핸들러!

### 5교시: 보호된 엔드포인트 ⭐⭐⭐

- **개념 (8min)**:
  - 인증 필요 API
  - Depends로 보호
  - 미인증 사용자 차단
- **Basic (20min)**:
  - 의존성으로 사용자 요구
  - 자동 문서의 자물쇠
  - 401 Unauthorized
- **Practice (12min)**:
  - 마이페이지 API
  - 게시글 작성 API
- **Exercise (10min)**:
  - 전체 API에 인증 적용

### 6교시: 인가 (Authorization) ⭐⭐⭐

- **개념 (10min)**:
  - 인증 vs 인가
  - 역할(Role)
  - RBAC
  - 권한 체크
- **Basic (22min)**:
  - User 모델에 role 추가
  - 권한 체크 의존성
  - admin만 접근 가능한 API
- **Practice (10min)**:
  - 관리자 권한 체크 구현
- **Exercise (8min)**:
  - 여러 역할 구현

### 7교시: CORS 설정 ⭐⭐

- **개념 (10min)**:
  - CORS란?
  - Origin
  - Preflight
  - 왜 필요한가?
- **Basic (20min)**:
  - CORSMiddleware
  - 허용 도메인
  - 허용 메서드
  - 실전 설정
- **Practice (12min)**:
  - CORS 설정
  - 프론트엔드 연동 준비
- **Exercise (8min)**:
  - 환경별 CORS 설정

### 8교시: Day 13 종합 실습

- **복습 퀴즈 (10min)**: OAuth2, 인가, CORS, 전역 에러
- **🟢 기초 Problem (15min)**: OAuth2 인증 적용
- **🟡 응용 Problem (15min)**: 역할 기반 권한 (user/admin)
- **🔴 도전 Problem (10min)**: 복잡한 권한 로직

---

## Day 14: 로깅, 미들웨어, 비동기, 테스팅 ⭐⭐⭐

### 1교시: Day 13 복습 + 로깅 기초 시작 ✨

- **복습 퀴즈 (10min)**: OAuth2, 인가, CORS
- **핵심 복습 (15min)**:
  - 권한 체크 재구현
  - 전역 에러 핸들러 복습
  - 간단한 Q&A
- **로깅 기초 시작 (25min)**:
  - 개념 (12min):
    - 로깅의 중요성 (프로덕션 필수!)
    - print() vs logging
    - 로그 레벨 (DEBUG, INFO, WARNING, ERROR, CRITICAL)
    - 디버깅과 모니터링
  - Basic (13min):
    ```python
    import logging
    
    logging.basicConfig(
        level=logging.INFO,
        format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
        handlers=[
            logging.FileHandler("app.log"),
            logging.StreamHandler()
        ]
    )
    
    logger = logging.getLogger(__name__)
    logger.info("User created")
    logger.error("Database error")
    ```

### 2교시: 로깅 기초 ⭐⭐⭐

- **Basic 완성 (25min)**:
  - 로그 레벨 설정
  - 파일 로깅
  - 포맷 설정
  - 실전 예제
- **Practice (15min)**:
  - FastAPI에서 로거 사용
  - 엔드포인트별 로깅
- **Exercise (10min)**:
  - 에러 로깅 추가
  - 요청/응답 로깅

> **중요**: 프로덕션 레벨이라면 로깅은 필수!

### 3교시: 로깅 실전 ⭐⭐⭐ ✨ NEW!

- **개념 (10min)**:
  - 프로덕션 로깅 전략
  - 로그 레벨 선택 기준
  - 로그 파일 관리
  - 로그 분석
- **Basic (22min)**:
  - 로그 파일 로테이션:
    ```python
    from logging.handlers import RotatingFileHandler
    
    handler = RotatingFileHandler(
        "app.log",
        maxBytes=10*1024*1024,  # 10MB
        backupCount=5
    )
    ```
  - 여러 핸들러 동시 사용
  - 에러 로깅 + 스택 트레이스:
    ```python
    try:
        # 코드
    except Exception as e:
        logger.exception("Error occurred")  # 스택 포함!
    ```
  - 요청 ID 추가 (미들웨어 연계)
- **Practice (10min)**:
  - 로그 전략 수립
  - 실전 로깅 구현
- **Exercise (8min)**:
  - 프로덕션 로깅 시스템 구축

> **중요 추가**: 로깅 실전 50분 확보!

### 4교시: 커스텀 미들웨어 ⭐⭐ ✨ NEW!

- **개념 (10min)**:
  - 미들웨어란?
  - 요청/응답 전처리
  - 실전 활용 사례
  - CORS 미들웨어 복습
- **Basic (22min)**:
  ```python
  from fastapi import Request
  import time
  import logging
  import uuid
  
  @app.middleware("http")
  async def log_requests(request: Request, call_next):
      # 요청 ID 생성
      request_id = str(uuid.uuid4())
      request.state.request_id = request_id
      
      # 요청 로깅
      logger.info(
          f"[{request_id}] {request.method} {request.url.path}",
          extra={"request_id": request_id}
      )
      
      # 실행 시간 측정
      start_time = time.time()
      response = await call_next(request)
      process_time = time.time() - start_time
      
      # 응답 로깅
      logger.info(
          f"[{request_id}] Completed in {process_time:.2f}s "
          f"Status: {response.status_code}",
          extra={"request_id": request_id, "duration": process_time}
      )
      
      # 커스텀 헤더 추가
      response.headers["X-Request-ID"] = request_id
      response.headers["X-Process-Time"] = str(process_time)
      
      return response
  ```
  - 실행 시간 측정
  - 요청 로깅
  - CORS 미들웨어 (복습)
- **Practice (10min)**:
  - 로깅 미들웨어 구현
  - 요청 ID 추적
- **Exercise (8min)**:
  - 인증 미들웨어
  - 커스텀 헤더 추가

> **중요 추가**: 커스텀 미들웨어 50분 확보!

### 5교시: 비동기 + httpx ⭐⭐

- **개념 (10min)**:
  - 블로킹 vs 논블로킹
  - 동시성
  - I/O 대기 시간
  - FastAPI와 비동기
  - **언제 사용하나?** (핵심!)
    - 외부 API 호출
    - DB 쿼리 (많은 경우)
    - 파일 I/O
- **Basic (22min)**:
  - async def, await 기초
  - httpx 설치 및 사용
  - AsyncClient
  - 외부 API 호출
  - 여러 요청 동시 처리
- **Practice (10min)**:
  - 비동기 API 호출 구현
- **Exercise (8min)**:
  - 여러 외부 API 동시 호출

> **중요**: 깊이보다 "왜 필요한가?" 중심!

### 6교시: 백그라운드 태스크 ⭐⭐

- **개념 (10min)**:
  - BackgroundTasks
  - 비동기 작업 처리
  - 사용 사례
- **Basic (20min)**:
  - BackgroundTasks 사용
  - 이메일 전송 예시
  - 로그 기록
  - 파일 처리
- **Practice (12min)**:
  - 백그라운드 작업 구현
- **Exercise (8min)**:
  - 이미지 처리 백그라운드

### 7교시: 테스팅 기초 ⭐⭐⭐

- **개념 (12min)**:
  - 테스트의 중요성 (프로덕션 필수!)
  - pytest 소개
  - 단위 테스트 vs 통합 테스트
  - FastAPI TestClient
- **Basic (20min)**:
  - pytest 설치
  - 테스트 함수 작성
  - TestClient 사용
  - 기본 assert
  ```python
  from fastapi.testclient import TestClient
  from main import app
  
  client = TestClient(app)
  
  def test_read_main():
      response = client.get("/")
      assert response.status_code == 200
      assert response.json() == {"message": "Hello"}
  
  def test_create_user():
      response = client.post("/users", json={"name": "test"})
      assert response.status_code == 201
  ```
- **Practice (10min)**:
  - 간단한 엔드포인트 테스트
  - CRUD 테스트
- **Exercise (8min)**:
  - 기존 API에 테스트 추가

> **중요**: 프로덕션 레벨이라면 테스팅 필수!

### 8교시: 테스팅 실전 + 파일 처리 ⭐⭐⭐ ✨ 확대!

- **테스팅 실전 (30min)**: ✨ NEW!
  - 개념 (5min):
    - fixture
    - 테스트 DB 분리
    - 인증 테스트
  - Basic (15min):
    ```python
    import pytest
    from fastapi.testclient import TestClient
    import sqlite3
    
    @pytest.fixture
    def client():
        return TestClient(app)
    
    @pytest.fixture
    def test_db():
        # 테스트용 DB 생성
        conn = sqlite3.connect(":memory:")
        cursor = conn.cursor()
        # 테이블 생성
        cursor.execute("""
            CREATE TABLE users (
                id INTEGER PRIMARY KEY,
                email TEXT,
                password TEXT
            )
        """)
        conn.commit()
        yield conn
        conn.close()
    
    def test_create_user(client, test_db):
        response = client.post(
            "/users",
            json={"email": "test@example.com", "password": "test123"}
        )
        assert response.status_code == 201
    
    def test_with_auth(client):
        # 1. 로그인
        login_response = client.post(
            "/login",
            json={"email": "admin@test.com", "password": "admin"}
        )
        token = login_response.json()["access_token"]
        
        # 2. 인증된 요청
        response = client.get(
            "/me",
            headers={"Authorization": f"Bearer {token}"}
        )
        assert response.status_code == 200
        assert response.json()["email"] == "admin@test.com"
    ```
  - Practice (7min):
    - fixture 사용
    - 인증 테스트 작성
  - Exercise (3min):
    - 통합 테스트 작성

- **파일 처리 (20min)**:
  - 업로드 (10min):
    - UploadFile 기본
    - 파일 저장
    - 크기/타입 검증
  - 다운로드 (10min):
    - FileResponse 사용
    - Content-Disposition

> **중요 확대**: 테스팅 실전 30분 확보!

---

## Day 15: 최종 프로젝트 ⭐⭐⭐

### 1교시: Day 14 복습 + 프로젝트 킥오프 ✨

- **복습 퀴즈 (10min)**: 로깅, 미들웨어, 테스팅
- **핵심 복습 (15min)**:
  - 미들웨어 복습
  - pytest 복습
  - 간단한 Q&A
- **프로젝트 안내 (25min)**:
  - 요구사항 (10min):
    - 기능 목록
    - **필수**: 로깅, 기본 테스트 포함
    - 평가 기준
  - 예시 프로젝트 (10min):
    - TODO API with Auth
    - 블로그 API
    - 쇼핑몰 API
  - 시간 배분 전략 (5min)

### 2교시: 프로젝트 기획 및 설계 ⭐⭐⭐

- **요구사항 분석 (20min)**:
  - 기능 목록 작성
  - 우선순위 결정 (MVP)
  - 로깅 전략
  - 테스트 범위
- **API 설계 (20min)**:
  - 엔드포인트 설계
  - Request/Response 모델
- **DB 스키마 설계 (10min)**:
  - 테이블 구조
  - 관계 설정

### 3교시: 프로젝트 구현 (1) - 기본 구조 ⭐⭐⭐

- **프로젝트 초기화 (15min)**:
  - 디렉터리 구조 (3계층)
  - 가상환경
  - 설정 파일 (.env)
  - 로거 설정
- **DB 모델 작성 (20min)**:
  - 테이블 생성
  - 초기 데이터
- **기본 CRUD (15min)**:
  - 핵심 엔드포인트 구현

### 4교시: 프로젝트 구현 (2) - 인증 적용 ⭐⭐⭐

- **사용자 모델 (15min)**:
  - User 테이블
  - 패스워드 해싱
- **인증 구현 (25min)**:
  - 회원가입
  - 로그인
  - JWT
- **보호 적용 (10min)**:
  - 인증 필요 API에 적용

### 5교시: 프로젝트 구현 (3) - 핵심 기능 및 마무리 ⭐⭐⭐

- **핵심 기능 구현 (25min)**:
  - 주요 비즈니스 로직
  - Service 계층 활용
  - 검증 강화
  - 로깅 추가
- **테스트 작성 (20min)**:
  - 주요 엔드포인트 테스트
  - pytest 실행
- **코드 정리 (5min)**:
  - 리팩토링
  - 주석 추가

### 6교시: 프로젝트 발표 준비 + 발표 (1) ⭐⭐⭐

- **발표 준비 (10min)**:
  - 시연 순서
  - 포인트 정리
- **발표 1-2팀 (40min)**:
  - 각 팀 20min
  - 시연: 8-10min
  - 설명: 6-8min
  - 질의응답: 4-6min

### 7교시: 프로젝트 발표 (2) ⭐⭐⭐

- **발표 3-4팀 (40min)**:
  - 각 팀 20min
  - 시연: 8-10min
  - 설명: 6-8min
  - 질의응답: 4-6min
- **중간 회고 (10min)**:
  - 배운 점 공유
  - 질문 및 피드백

### 8교시: 프로젝트 발표 (3) + 전체 마무리 ⭐⭐⭐

- **발표 5-6팀 (40min)**:
  - 각 팀 20min
  - 시연: 8-10min
  - 설명: 6-8min
  - 질의응답: 4-6min
- **전체 회고 (10min)**:
  - 베스트 프로젝트 선정
  - 전체 소감
  - 향후 학습 방향

> **참고**: 6팀 이상이면 각 팀 발표 시간 15min으로 조정!

---

## 📌 핵심 학습 목표 (프로덕션 레벨)

### 최우선 항목 ⭐⭐⭐

1. **프로젝트 구조**: 계층 분리 (Web-Service-Data)
2. **의존성 주입**: FastAPI Depends 마스터
3. **JWT 인증**: 회원가입, 로그인, 토큰 검증
4. **OAuth2 패턴**: 표준 인증 구현
5. **권한 관리**: 역할 기반 접근 제어
6. **환경 변수**: 설정 관리, 보안
7. **로깅**: 기초 + 실전 (프로덕션 필수!)
8. **테스팅**: 기초 + 실전 (프로덕션 필수!)
9. **전역 에러 핸들러**: 일관된 에러 응답 (추가!)
10. **커스텀 미들웨어**: 요청/응답 처리 (추가!)

### 중요 항목 ⭐⭐

1. 비동기 프로그래밍 (개념 이해)
2. CORS 설정
3. 파일 업로드/다운로드
4. 백그라운드 태스크

### 기본 항목 ⭐

1. httpx 활용
2. 성능 최적화 개념

---

## 📝 v7.0 주요 변경사항

1. ✅ **1교시 복습 간소화**: 10min 퀴즈 + 15min 복습 + 25min 진도
2. ✅ **Day 11-7교시**: 계층 분리 통합 (기본+심화 50min)
3. ✅ **Day 12-1교시**: 인증 개념으로 변경 (계층 분리 심화 제거)
4. ✅ **Day 13-4교시**: 전역 에러 핸들러 추가 (20min)
5. ✅ **Day 14-3교시**: 로깅 실전 추가 (50min)
6. ✅ **Day 14-4교시**: 커스텀 미들웨어 추가 (50min)
7. ✅ **Day 14-8교시**: 테스팅 실전 추가 (30min)
8. ✅ 프로덕션 레벨 완성도 대폭 향상!
9. ✅ **총 100min 시간 확보** (심화 과정에서)

---

## 🎓 학습 후 다음 단계

### 권장 학습 주제

1. **SQLAlchemy ORM** (선택):
   - raw SQL → ORM 전환
   - 관계 매핑
   - 마이그레이션

2. **심화 테스팅**:
   - 테스트 커버리지
   - Mock/Stub
   - 통합 테스트

3. **배포**:
   - Docker
   - CI/CD
   - 클라우드 (AWS, GCP)

4. **모니터링**:
   - 로그 분석
   - 성능 모니터링
   - 알림 시스템

---
