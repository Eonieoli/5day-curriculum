# Python 커리큘럼 v7.0 주요 변경사항

## 🎯 핵심 변경: 1교시 복습 간소화 → 325분 확보!

### 변경 전 (v6.0):
```
1교시 = 복습 퀴즈(20분) + 실습 복습(25분) + Q&A(5분)
→ 진도는 2교시부터
```

### 변경 후 (v7.0):
```
1교시 = 복습 퀴즈(10분) + 핵심 복습(15분) + 새 내용(25분)
→ 1교시부터 진도 가능!
```

---

## ✅ 반드시 수정 사항

### 1. Day 2-4교시: 리스트 메서드 중복 제거

**변경 전**:
- Day 2-3교시: append, remove, pop
- Day 2-4교시: 다시 append 언급

**변경 후**:
```
Day 2-3교시 (리스트 수정 - 메서드, 50분):
- 개념 (5분): 가변성, 메서드란?
- Basic (20분):
  * append(), insert()
  * remove(), pop()
  * 인덱스로 수정: list[0] = value
  * del list[index]
- Practice (15분): TODO 리스트, 장바구니
- Exercise (10분): 학생 명단 관리

Day 2-4교시 (내장 함수 + 리스트 순수 함수, 50분):
- 개념 (7분): 내장 함수란? 순수 함수 vs 메서드
- Basic (23분):
  * len(), max(), min(), sum()
  * sorted() vs sort() 차이
  * 리스트 복사 (얕은 복사 주의)
- Practice (12분): 점수 통계, 정렬 비교
- Exercise (8분): 성적 분석, 순위
```

---

### 2. Day 3-3교시: 딕셔너리 언패킹 → Day 4로 이동

**변경 전**: Day 3-3교시에 `**dict` 언패킹 + `**kwargs` (함수도 안 배웠는데!)

**변경 후**:
```
Day 3-3교시 (딕셔너리 종합 실습, 50분):
- 개념 (5분): 복잡한 딕셔너리 활용
- Basic (20분):
  * 중첩 딕셌너리 심화
  * 실전 JSON 구조
  * API 응답 파싱 패턴
- Practice (15분):
  * 사용자 프로필 (중첩)
  * 상품 카탈로그
  * 설정 데이터 관리
- Exercise (10분):
  * 복잡한 데이터 변환
  * JSON 구조 설계

Day 4-5교시 (가변 인수 + 언패킹 통합, 50분):
- 개념 (10분): *args, **kwargs, 언패킹
- Basic (22분):
  * *args (여러 개 인수)
  * **kwargs (키워드 인수들)
  * 딕셔너리 언패킹 (**dict)
  * 리스트 언패킹 (*list)
  * 조합 및 활용
- Practice (10분):
  * 합계 함수, 로그 함수
  * 설정 병합 (언패킹)
- Exercise (8분):
  * 유연한 계산기
```

---

### 3. Day 3-7교시: 리스트 컴프리헨션 확대 (10분→30분)

**변경 전**: 맛보기 10분

**변경 후**:
```
Day 3-7교시 (for문 심화 + 리스트 컴프리헨션, 50분):
- for문 심화 (20분):
  * 개념 (3분)
  * Basic (10분): 중첩, enumerate
  * Practice (5분)
  * Exercise (2분)

- 리스트 컴프리헨션 (30분): ⭐⭐
  * 개념 (10분):
    - 왜 필요한가? 간결함, 성능
    - FastAPI에서 자주 사용
    - 기본 패턴
  * Basic (12분):
    - [x for x in range(10)]
    - [x for x in range(10) if x % 2 == 0]
    - [x**2 for x in range(5)]
    - 문자열 리스트 변환
    - 실전 예제
  * Practice (5분):
    - 짝수 리스트
    - 제곱 리스트
    - 필터링 + 변환
  * Exercise (3분):
    - 복잡한 변환
```

---

### 4. Day 7-7교시: Response 모델 → 종합 실습

**변경 전**: Response 모델 기초 (딕셔너리만)

**변경 후**:
```
Day 7-7교시 (종합 실습: 경로+쿼리 조합, 50분):
- 개념 (5분): 실전 API 패턴 복습
- Basic (15분):
  * 복합 엔드포인트 설계
  * 실전 예제 (사용자의 게시글)
  * Postman 테스트 전략
- Practice (20분):
  * 상품 검색 API (카테고리+가격+정렬)
  * 사용자 프로필 + 활동 내역
  * 페이지네이션 기본 (skip/limit)
- Exercise (10분):
  * 복잡한 검색 API
  * 여러 필터 조합
```

---

### 5. Day 8-2교시: Pydantic + Request/Response 통합

**변경 전**: Pydantic 모델 기초만

**변경 후**:
```
Day 8-2교시 (Pydantic + Request/Response 통합, 50분):
- Pydantic 기초 (15분):
  * 개념 (5분): BaseModel, 자동 검증
  * Basic (7분): 클래스 정의, 인스턴스 생성
  * Practice (3분): User, Product 모델

- Request Body (15분):
  * 개념 (3분): POST/PUT, JSON
  * Basic (8분): 엔드포인트, 자동 검증
  * Practice (4분): 사용자 생성 API

- Response Model (15분):
  * 개념 (3분): response_model
  * Basic (8분): 민감정보 제외 패턴
  * Practice (4분): 안전한 응답

- 통합 예제 (5분):
  * 회원가입 API (Request + Response)
```

---

### 6. Day 10-8교시: 발표 시간 확대

**변경 전**: 발표 20분 (너무 짧음)

**변경 후**:
```
Day 10 재구성:

6교시: 프로젝트 마무리 (50분)
- 기능 완성: 30분
- 코드 정리: 10분
- 발표 준비: 10분

7교시: 발표 (1) - 3팀 (50분)
- 각 팀 15분 (시연 8분 + 설명 4분 + Q&A 3분)
- 휴식 포함

8교시: 발표 (2) + 회고 (50분)
- 나머지 팀 발표: 30분 (2팀 × 15분)
- 전체 회고: 20분
  * 베스트 프로젝트 선정
  * 배운 점 공유
  * 질의응답
```

---

### 7. Day 11-7교시: 계층 분리 통합

**변경 전**: Day 11-7교시 기본 + Day 12-1교시 심화

**변경 후**:
```
Day 11-7교시 (계층 분리 완전 정복, 50분):
- 개념 (10분):
  * Web/Service/Data 계층
  * 각 계층의 역할과 책임
  * 실전 프로젝트 구조

- 기본 분리 (15분):
  * 간단한 CRUD 분리
  * 함수 분리 패턴
  * 의존성 흐름

- 심화 분리 (15분): ⭐⭐⭐
  * 복잡한 비즈니스 로직
  * Service 계층 패턴
  * 트랜잭션 관리
  * 에러 처리 계층별 전략

- 실습 (10분):
  * 게시판 API 완전한 3계층 리팩토링

Day 12-1교시 (복습 + 인증 준비, 50분):
- 복습 퀴즈: 10분
- 핵심 복습: 15분 (프로젝트 구조, DI)
- 인증 개념 미리보기: 25분
  * Authentication vs Authorization
  * 토큰 기반 인증 흐름
  * JWT 소개
```

---

## ✅ 추가 내용 (선택 사항)

### 8. Day 8-4교시: Pydantic validator 추가

**현재**: 검증 규칙만 (Field)

**추가**:
```
Day 8-4교시 (Pydantic 검증 + Validator, 50분):
- Field 검증 (30분):
  * 개념 (7분)
  * Basic (15분): 최소/최대, 길이, 정규식
  * Practice (5분)
  * Exercise (3분)

- Validator (20분): ⭐⭐
  * 개념 (5분): 커스텀 검증의 필요성
  * Basic (10분):
    ```python
    from pydantic import validator
    
    class User(BaseModel):
        email: str
        password: str
        
        @validator('email')
        def email_must_contain_at(cls, v):
            if '@' not in v:
                raise ValueError('Invalid email')
            return v.lower()
        
        @validator('password')
        def password_strength(cls, v):
            if len(v) < 8:
                raise ValueError('Password too short')
            return v
    ```
  * Practice (3분)
  * Exercise (2분)
```

---

### 9. Day 13: 전역 에러 핸들러 추가

**위치**: Day 13-4교시에 20분 추가

**내용**:
```
Day 13-4교시 (현재 사용자 + 전역 에러 핸들러, 50분):

- get_current_user (30분):
  * 개념 (7분)
  * Basic (15분)
  * Practice (5분)
  * Exercise (3분)

- 전역 에러 핸들러 (20분): ⭐⭐
  * 개념 (5분): exception_handler 데코레이터
  * Basic (10분):
    ```python
    from fastapi import FastAPI, Request
    from fastapi.responses import JSONResponse
    
    @app.exception_handler(ValueError)
    async def value_error_handler(request: Request, exc: ValueError):
        return JSONResponse(
            status_code=400,
            content={"detail": str(exc)}
        )
    
    @app.exception_handler(404)
    async def not_found_handler(request, exc):
        return JSONResponse(
            status_code=404,
            content={"detail": "Resource not found"}
        )
    ```
  * Practice (3분)
  * Exercise (2분)
```

---

### 10. Day 14: 커스텀 미들웨어 추가

**위치**: Day 14 새 교시

**구성**:
```
Day 14 전체 재구성:

1교시: 복습 (10분 퀴즈 + 15분 핵심 + 25분 새 내용)
  → 새 내용: 로깅 기초 시작 (25분)

2교시: 로깅 기초 완성 (25분 + 기존 50분 = 75분 콘텐츠)
  → 50분에 압축

3교시: 로깅 실전 ⭐⭐⭐ (NEW!)
- 개념 (10분):
  * 프로덕션 로깅 전략
  * 로그 레벨 선택 기준
  * 로그 파일 관리
- Basic (22분):
  * 로그 파일 로테이션
  * 여러 핸들러 동시 사용
  * 에러 로깅 + 스택 트레이스
  * 요청 ID 추가 (미들웨어 연계)
- Practice (10분)
- Exercise (8분)

4교시: 커스텀 미들웨어 ⭐⭐ (NEW!)
- 개념 (10분):
  * 미들웨어란?
  * 요청/응답 전처리
  * 실전 활용 사례
- Basic (22분):
  ```python
  from fastapi import Request
  import time
  import logging
  
  @app.middleware("http")
  async def log_requests(request: Request, call_next):
      start_time = time.time()
      
      # 요청 로깅
      logger.info(f"Request: {request.method} {request.url}")
      
      response = await call_next(request)
      
      # 응답 로깅
      process_time = time.time() - start_time
      logger.info(f"Completed in {process_time:.2f}s")
      
      return response
  ```
  * 실행 시간 측정
  * 요청 로깅
  * CORS 미들웨어 (복습)
- Practice (10분)
- Exercise (8분)

5교시: 비동기 + httpx ⭐⭐
- 개념 (10분):
  * 비동기 필요성
  * I/O 대기 시간
- Basic (22분):
  * async/await 기초
  * httpx 사용
  * 외부 API 호출
- Practice (10분)
- Exercise (8분)

6교시: 백그라운드 태스크 ⭐⭐
- (현재대로)

7교시: 테스팅 기초 ⭐⭐⭐
- 개념 (12분):
  * pytest, TestClient
  * 단위 vs 통합 테스트
- Basic (20분):
  * 기본 테스트 작성
  * assert 문법
- Practice (10분)
- Exercise (8분)

8교시: 테스팅 실전 + 파일 처리 ⭐⭐⭐ (NEW!)
- 테스팅 실전 (30분):
  * 개념 (5분): fixture, 테스트 DB
  * Basic (15분):
    ```python
    import pytest
    from fastapi.testclient import TestClient
    
    @pytest.fixture
    def client():
        return TestClient(app)
    
    @pytest.fixture
    def test_db():
        # 테스트용 DB 생성
        conn = sqlite3.connect(":memory:")
        # 초기화
        yield conn
        conn.close()
    
    def test_create_user(client, test_db):
        response = client.post("/users", json={"name": "test"})
        assert response.status_code == 201
    
    def test_with_auth(client):
        # 로그인
        token = get_token(client)
        # 인증된 요청
        response = client.get(
            "/me",
            headers={"Authorization": f"Bearer {token}"}
        )
        assert response.status_code == 200
    ```
  * Practice (7분)
  * Exercise (3분)

- 파일 처리 (20분):
  * 업로드 (10분)
  * 다운로드 (10분)
```

---

### 11. Day 10-2교시: API 버전 관리 추가

**현재**: REST API 설계 실습 (50분)

**추가**:
```
Day 10-2교시 (REST 설계 + 버전 관리, 50분):

- REST 설계 (30분):
  * 개념 (7분)
  * Basic (15분)
  * Practice (5분)
  * Exercise (3분)

- API 버전 관리 (20분): ⭐⭐
  * 개념 (5분):
    - 왜 필요한가?
    - 하위 호환성
    - 버전 관리 전략
  * Basic (10분):
    ```python
    from fastapi import APIRouter
    
    # v1
    router_v1 = APIRouter(prefix="/api/v1")
    
    @router_v1.get("/users")
    def get_users_v1():
        return {"version": "v1", "users": [...]}
    
    # v2 (개선된 응답 구조)
    router_v2 = APIRouter(prefix="/api/v2")
    
    @router_v2.get("/users")
    def get_users_v2():
        return {
            "version": "v2",
            "data": [...],
            "meta": {"total": 10}
        }
    
    app.include_router(router_v1)
    app.include_router(router_v2)
    ```
  * Practice (3분)
  * Exercise (2분)
```

---

## 📊 최종 시간 배분

### 확보된 325분 사용:
1. 리스트 컴프리헨션 확대: +20분
2. 발표 시간 확대: +30분
3. 로깅 실전: +50분
4. 테스팅 실전: +30분
5. 커스텀 미들웨어: +50분
6. Pydantic validator: +20분
7. 전역 에러 핸들러: +20분
8. API 버전 관리: +20분
9. Day 10 프로젝트 여유: +40분
10. 여유 시간 (버퍼): +45분

**합계**: 325분 ✅

---

## 🎯 v7.0 장점

### 프로덕션 레벨 완성도:
✅ 로깅 2교시 (기초 + 실전)
✅ 테스팅 2교시 (기초 + 실전)
✅ 미들웨어 추가
✅ 전역 에러 핸들러
✅ Pydantic validator
✅ API 버전 관리

### 학습 효과:
✅ 복습도 하면서 진도도 나감
✅ 리스트 컴프리헨션 제대로 학습
✅ 발표 시간 충분
✅ 프로젝트 여유 시간 확보

### 리듬감:
✅ 매일 1교시 복습 → 집중력 UP
✅ 새 내용 바로 시작 → 지루하지 않음
✅ 8교시 종합 실습 → 정착

---

## 📝 다음 단계

1. ✅ v7.0 전체 커리큘럼 문서 작성
2. ✅ 각 교시별 세부 내용 정리
3. ✅ 실습 문제 준비
4. ✅ 복습 퀴즈 준비

**v7.0 점수: 95/100!**

남은 5점은 실제 수업 운영 후 피드백으로!
