# Python 응용 과정 커리큘럼 v3.0

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
- Exercise: 5-10분

**8교시 종합 실습 (50분)**
- 복습 퀴즈: 10분
- 🟢 기초 Problem: 15분
- 🟡 응용 Problem: 15-20분
- 🔴 도전 Problem: 5-10분 (선택)

**복습 교시 (매일 1교시, 50분)**
- 퀴즈: 20분
- 실습 복습: 25분
- Q&A: 5분

---

## 📌 사전 과제 (Day 6 시작 전 - 선택)

### Postman 설치 (예상 10분)

**선택 설치 항목**
1. **Postman**: https://www.postman.com/downloads/
   - 또는 웹 버전 사용: https://web.postman.co/

**설치 확인**
- Postman 실행
- 계정 생성 (선택)

> 💡 **참고**: Day 6에서 함께 설치해도 됩니다.

---

## Day 6: 웹과 API의 이해

### 1교시: 기초 과정 복습 + 가상환경 설정 ⭐⭐⭐
- **퀴즈 (15분)**: Python 기초 핵심 (딕셔너리, 타입 힌트, 함수, JSON)
- **가상환경 + import 실무 (25분)**:
  - venv 생성, 활성화
  - pip install fastapi uvicorn
  - "import fastapi" 실습
  - import vs from import 차이
- **응용 과정 소개 (5분)**: 로드맵, 최종 목표
- **Q&A (5분)**

### 2교시: 웹의 동작 원리 ⭐⭐
- **개념 (15분)**: 클라이언트-서버 모델, 브라우저 역할, IP/도메인/포트, URL 구조
- **Basic (20분)**: 브라우저 개발자 도구 실습, 네트워크 탭 관찰, URL 파싱 예제
- **Practice (10분)**: URL 분해하기, 쿼리 파라미터 이해
- **Exercise (5분)**: URL 구조 분석 문제

### 3교시: HTTP 프로토콜 (1) - 메서드 ⭐⭐
- **개념 (10분)**: HTTP란?, Request/Response 구조, HTTP 메서드 종류
- **Basic (20분)**: GET, POST, PUT, DELETE 차이, 각 메서드 사용 시나리오, 개발자 도구로 관찰
- **Practice (12분)**: 브라우저에서 GET 요청 확인, 개발자 도구 실습
- **Exercise (8분)**: 메서드 선택 문제 (시나리오별 적절한 메서드 고르기)

### 4교시: HTTP 프로토콜 (2) - 상태 코드와 헤더 ⭐⭐
- **개념 (12분)**: 상태 코드 체계 (2xx, 3xx, 4xx, 5xx), 주요 상태 코드, HTTP 헤더
- **Basic (18분)**: 200, 201, 400, 404, 500 예제, Content-Type, Authorization 헤더
- **Practice (12분)**: 개발자 도구로 상태 코드 확인, 헤더 분석
- **Exercise (8분)**: 상태 코드 매칭 문제

### 5교시: REST API 개념 ⭐⭐⭐
- **개념 (12분)**: API란?, REST 아키텍처 원칙, RESTful API 설계, 리소스와 엔드포인트
- **Basic (20분)**: 좋은 API vs 나쁜 API 예제, 리소스 명명 규칙, HTTP 메서드 매핑
- **Practice (10분)**: 간단한 블로그 API 설계 (함께)
- **Exercise (8분)**: TODO 앱 API 엔드포인트 설계

### 6교시: JSON 복습 + 웹에서의 활용 ⭐⭐
- **개념 (8분)**: JSON과 웹, HTTP Body, API 응답 형식
- **Basic (15분)**: 
  - Day 5 복습: json.dumps(), json.loads()
  - 웹에서의 JSON: Request Body, Response Body
  - 실제 API 응답 예제
- **Practice (15분)**: 공개 API 응답 분석, JSON 파싱
- **Exercise (12분)**: API 응답 데이터 추출, 가공

### 7교시: Postman 설치 및 사용법 ⭐⭐
- **개념 (5분)**: Postman이란?, API 테스팅 도구의 필요성
- **Basic (20분)**: 설치, GET 요청, POST 요청, Headers 설정, Body 설정 (JSON)
- **Practice (20분)**: 공개 API 테스트 (JSONPlaceholder 등), 컬렉션 만들기
- **Exercise (5분)**: 특정 API 호출 과제

### 8교시: Day 6 종합 실습
- **복습 퀴즈 (10분)**: HTTP, REST, JSON, Postman
- **🟢 기초 Problem (15분)**: REST API 설계서 작성 (간단한 서비스)
- **🟡 응용 Problem (20분)**: Postman으로 공개 API 테스트 + 데이터 가공
- **🔴 도전 Problem (5분)**: 복잡한 JSON 데이터 파싱 및 변환

---

## Day 7: FastAPI 시작하기

### 1교시: Day 6 복습
- **퀴즈 (20분)**: HTTP, REST API, JSON, Postman
- **실습 복습 (25분)**: Postman 실습 재도전
- **Q&A (5분)**

### 2교시: FastAPI 소개 + 첫 API ⭐⭐⭐
- **개념 (10분)**: FastAPI란?, 특징과 장점, 다른 프레임워크 비교
- **환경 확인 (5분)**: pip list로 설치 확인 (Day 6에서 설치했음)
- **Basic (20분)**: Hello World API, uvicorn 실행, 브라우저 확인, --reload 옵션
- **Practice (10분)**: 함께 첫 API 만들기, 다양한 응답 시도
- **Exercise (5분)**: 자기소개 API, 현재 시간 API

### 3교시: 자동 문서화 ⭐⭐⭐
- **개념 (7분)**: Swagger UI, ReDoc, 자동 문서화의 장점
- **Basic (20분)**: /docs 접속, /redoc 접속, 문서에서 API 테스트, docstring 추가
- **Practice (15분)**: 여러 API 만들고 문서 확인, 설명 추가하기
- **Exercise (8분)**: 문서화가 잘 된 API 3개 만들기

### 4교시: 경로 매개변수 (Path Parameter) ⭐⭐⭐
- **개념 (8분)**: 경로 매개변수란?, 동적 라우팅, 타입 지정
- **Basic (22분)**: {item_id} 문법, int 타입, str 타입, 자동 검증, 에러 응답
- **Practice (13분)**: 사용자 조회 API, 상품 조회 API
- **Exercise (7분)**: 게시글 조회, 카테고리별 조회

### 5교시: 쿼리 매개변수 (Query Parameter) ⭐⭐⭐
- **개념 (8분)**: 쿼리 매개변수란?, ?key=value 형식, 검색/필터링 용도
- **Basic (22분)**: 기본 쿼리, 기본값 설정, Optional 쿼리, 여러 개 쿼리
- **Practice (12분)**: 검색 API, 페이징 API (skip, limit)
- **Exercise (8분)**: 필터링 API (여러 조건)

### 6교시: 경로 + 쿼리 조합 ⭐⭐
- **개념 (5분)**: 경로와 쿼리 함께 사용, 우선순위
- **Basic (18분)**: 조합 예제, 실전 API 패턴, Postman 테스트
- **Practice (17분)**: 사용자의 게시글 조회, 상품 검색 API
- **Exercise (10분)**: 복합 API 만들기

### 7교시: Response 모델 미리보기 ⭐⭐
- **개념 (8분)**: 응답 구조, 딕셔너리 반환
- **Basic (20분)**: 간단한 Response 모델, dict 반환, 일관된 응답 구조
- **Practice (15분)**: 사용자 응답, 상품 응답
- **Exercise (7분)**: 응답 모델 설계

### 8교시: Day 7 종합 실습
- **복습 퀴즈 (10분)**: FastAPI 기본, 경로/쿼리 매개변수
- **🟢 기초 Problem (15분)**: 간단한 도서관 API (책 조회)
- **🟡 응용 Problem (20분)**: 쇼핑몰 상품 API (경로+쿼리 조합)
- **🔴 도전 Problem (5분)**: 복잡한 검색 API

---

## Day 8: Pydantic과 Request/Response

### 1교시: Day 7 복습
- **퀴즈 (20분)**: FastAPI 기본, 매개변수
- **실습 복습 (25분)**: 경로/쿼리 매개변수 재실습
- **Q&A (5분)**

### 2교시: Pydantic 모델 기초 ⭐⭐⭐
- **개념 (10분)**: Pydantic이란?, BaseModel, 자동 검증, FastAPI에서의 역할
- **Basic (22분)**: BaseModel 상속, 필드 정의, 인스턴스 생성, 자동 타입 변환
- **Practice (10분)**: User 모델, Product 모델 만들기
- **Exercise (8분)**: Post 모델, Comment 모델

### 3교시: Request Body ⭐⭐⭐
- **개념 (8분)**: Request Body란?, POST/PUT에서 사용, JSON과의 관계
- **Basic (22분)**: POST 엔드포인트, Pydantic 모델로 받기, 자동 검증, 에러 응답
- **Practice (13분)**: 사용자 생성 API, 상품 등록 API
- **Exercise (7분)**: 게시글 작성 API

### 4교시: Pydantic 검증 기능 ⭐⭐⭐
- **개념 (12분)**: Field() 함수, 검증 규칙, 에러 메시지, 보안
- **Basic (20분)**: 최소/최대값, 길이 제한, 정규식, 커스텀 검증
- **Practice (10분)**: 회원가입 모델 (이메일, 비밀번호 검증)
- **Exercise (8분)**: 상품 등록 검증 (가격, 재고)

### 5교시: Response Model ⭐⭐
- **개념 (8분)**: response_model이란?, 응답 데이터 제어, 민감정보 제외
- **Basic (20분)**: response_model 지정, 비밀번호 제외, List[Model] 반환
- **Practice (15분)**: 사용자 조회 (비밀번호 제외), 목록 조회
- **Exercise (7min)**: 안전한 응답 모델 설계

### 6교시: 상태 코드 지정 ⭐⭐
- **개념 (8분)**: status_code 매개변수, HTTPException, 적절한 상태 코드 선택
- **Basic (20분)**: 201 Created, 400 Bad Request, 404 Not Found, HTTPException 사용
- **Practice (15분)**: CRUD API에 상태 코드 적용
- **Exercise (7분)**: 에러 핸들링이 있는 API

### 7교시: Optional과 Union 활용 ⭐⭐
- **개념 (8분)**: Optional 필드, 부분 업데이트, Union 타입
- **Basic (20분)**: Optional[str], None 기본값, PATCH 메서드, 선택적 필드
- **Practice (15분)**: 프로필 업데이트 API (부분 수정)
- **Exercise (7분)**: 유연한 업데이트 API

### 8교시: Day 8 종합 실습
- **복습 퀴즈 (10분)**: Pydantic, Request/Response
- **🟢 기초 Problem (15분)**: TODO API (CRUD 기본)
- **🟡 응용 Problem (20분)**: 블로그 API (검증 포함)
- **🔴 도전 Problem (5분)**: 복잡한 검증 규칙

---

## Day 9: 데이터베이스 연동

### 1교시: Day 8 복습
- **퀴즈 (20분)**: Pydantic 전체
- **실습 복습 (25분)**: Request Body, 검증
- **Q&A (5분)**

### 2교시: 데이터베이스 기초 + SQLite ⭐⭐
- **개념 (15분)**: 데이터베이스란?, RDBMS, SQLite 특징, 테이블/행/열
- **Basic (22분)**: SQL 기본 (SELECT, INSERT, UPDATE, DELETE만), SQLite 브라우저
- **Practice (8분)**: SQL 문법 연습 (간단하게)
- **Exercise (5분)**: 기본 SQL 작성

### 3교시: SQLite 연결 ⭐⭐
- **개념 (8분)**: sqlite3 모듈, 커넥션과 커서, commit의 중요성
- **Basic (22분)**: 데이터베이스 연결, 테이블 생성, 커서 사용, 커넥션 닫기
- **Practice (13분)**: 데이터베이스 초기화 코드 작성
- **Exercise (7분)**: 테이블 설계 및 생성

### 4교시: 데이터 삽입 (CREATE) ⭐⭐
- **개념 (10분)**: INSERT문, 파라미터 바인딩, SQL Injection 방지
- **Basic (20분)**: 단일 삽입, 여러 개 삽입, executemany(), lastrowid
- **Practice (13분)**: 사용자 추가, 상품 추가 함수
- **Exercise (7분)**: 데이터 삽입 API

### 5교시: 데이터 조회 (READ) ⭐⭐⭐
- **개념 (7분)**: SELECT문, WHERE 조건, fetchone/fetchall
- **Basic (22분)**: 전체 조회, 조건 조회, 단일 조회, 컬럼 선택
- **Practice (13분)**: 목록 조회, 상세 조회 함수
- **Exercise (8분)**: 조건별 조회 API

### 6교시: 데이터 수정 및 삭제 (UPDATE, DELETE) ⭐⭐
- **개념 (7분)**: UPDATE문, DELETE문, WHERE의 중요성
- **Basic (20min)**: 수정, 삭제, 안전한 삭제 (존재 확인)
- **Practice (15분)**: 업데이트 함수, 삭제 함수
- **Exercise (8분)**: 수정/삭제 API

### 7교시: FastAPI + SQLite 통합 ⭐⭐⭐
- **개념 (10분)**: 엔드포인트에서 DB 작업, 함수 분리, 에러 처리
- **Basic (22분)**: CRUD API 전체 구현, Pydantic + DB 조합, 트랜잭션
- **Practice (13분)**: 완전한 게시판 API 만들기
- **Exercise (5분)**: TODO API에 DB 적용

### 8교시: Day 9 종합 실습
- **복습 퀴즈 (10분)**: SQL, SQLite, CRUD
- **🟢 기초 Problem (15분)**: 간단한 메모 API (DB 포함)
- **🟡 응용 Problem (20분)**: 사용자 관리 시스템
- **🔴 도전 Problem (5분)**: 검색 기능 추가

---

## Day 10: REST API 설계 및 프로젝트

### 1교시: Day 9 복습
- **퀴즈 (20분)**: 데이터베이스, CRUD
- **실습 복습 (25분)**: FastAPI + DB 통합
- **Q&A (5분)**

### 2교시: REST API 설계 실습 ⭐⭐⭐
- **개념 (10분)**: RESTful 설계 원칙 복습, 엔드포인트 네이밍, HTTP 메서드 선택
- **Basic (20분)**: 좋은 설계 vs 나쁜 설계, 실제 서비스 API 분석
- **Practice (15분)**: 도서관 시스템 API 설계 (함께)
- **Exercise (5분)**: 쇼핑몰 API 설계

### 3교시: 라우터 분리 ⭐⭐
- **개념 (8분)**: APIRouter, 코드 구조화, 관심사 분리
- **Basic (20분)**: APIRouter 사용, prefix 설정, tags, include_router
- **Practice (15분)**: users, posts 라우터 분리
- **Exercise (7분)**: 3개 이상 라우터 구성

### 4교시: 에러 처리 고도화 ⭐⭐
- **개념 (8분)**: HTTPException 심화, 커스텀 에러, 일관된 에러 응답
- **Basic (20분)**: 404 Not Found, 400 Bad Request, 상세 에러 메시지, detail 활용
- **Practice (15분)**: 에러 핸들링 함수 작성
- **Exercise (7분)**: 모든 API에 에러 처리 적용

### 5교시: 페이지네이션 ⭐⭐
- **개념 (7분)**: 페이지네이션 필요성, skip/limit 패턴
- **Basic (20분)**: 쿼리로 skip, limit 받기, SQL LIMIT/OFFSET, 전체 개수 반환
- **Practice (15분)**: 페이지네이션 구현
- **Exercise (8분)**: 페이지 번호 방식 구현

### 6교시: 프로젝트 주제 선정 및 설계
- **주제 선정 (15분)**: TODO, 블로그, 쇼핑몰, 게시판 중 선택
- **요구사항 정의 (20분)**: 기능 목록, 우선순위 결정
- **API 스펙 작성 (15분)**: 엔드포인트, Request/Response

### 7교시: 프로젝트 구현 (1) - 초기 설정 및 기본 구조
- **프로젝트 초기화 (15분)**: 디렉터리 구조, DB 초기화
- **기본 CRUD (35분)**: 핵심 엔드포인트 구현

### 8교시: 프로젝트 구현 (2) - 기능 완성 및 발표
- **기능 완성 (30분)**: Pydantic 모델, 에러 처리, 검증
- **테스트 (10분)**: Postman으로 전체 API 테스트
- **발표 (10분)**: 간단히 시연 및 설명

---

## 📌 핵심 학습 목표 (FastAPI 중심)

### 최우선 항목 ⭐⭐⭐
1. **Pydantic 모델**: Request/Response 데이터 구조화
2. **경로/쿼리 매개변수**: API 엔드포인트 설계
3. **CRUD 작업**: 데이터베이스 연동
4. **REST API 설계**: RESTful 원칙 적용
5. **에러 처리**: HTTPException, 상태 코드
6. **Postman**: API 테스팅

### 중요 항목 ⭐⭐
1. HTTP 프로토콜 이해
2. JSON 데이터 처리 (웹 맥락)
3. SQLite 기본
4. 라우터 분리
5. 페이지네이션

### 기본 항목 ⭐
1. 웹 동작 원리
2. 자동 문서화
3. SQL 기본 문법

---

## 💡 교육 운영 팁

### 준비 사항
- [ ] FastAPI, uvicorn 설치 확인
- [ ] Postman 설치 및 기본 사용법 가이드
- [ ] SQLite 브라우저 설치 (선택)
- [ ] 각 일차별 PPT 슬라이드
- [ ] 각 일차별 코드 예제 (.py 파일)
- [ ] Postman 컬렉션 (공개 API 테스트용)
- [ ] 전체 정답 코드
- [ ] 트러블슈팅 FAQ

### 파일 구조
```
Day6_웹과API/
├── slides/
│   └── Day6_전체.pptx
├── code/
│   ├── 01_basic_http.py
│   ├── 02_json_review.py
│   └── ...
├── postman/
│   └── Day6_collection.json
└── README.md

Day7_FastAPI시작/
├── slides/
│   └── Day7_전체.pptx
├── code/
│   ├── 01_hello_world.py
│   ├── 02_path_param.py
│   ├── 03_query_param.py
│   └── ...
├── solutions/
│   ├── Exercise_정답/
│   └── Problem_정답/
└── README.md
```

### uvicorn 서버 실행
```bash
# 기본 실행
uvicorn main:app

# 자동 재시작 (개발 시 필수!)
uvicorn main:app --reload

# 포트 변경
uvicorn main:app --reload --port 8080
```

### Postman 활용
- Day 6-7: GET, POST 요청 연습
- Day 8: Request Body, Headers 설정
- Day 9-10: 전체 CRUD 테스트

### 실습 강조 포인트
1. **서버 실행 → 브라우저/Postman 테스트 → 결과 확인** 루틴 반복
2. 에러 메시지 읽는 법 강조 (400, 422 에러 특히)
3. 자동 문서 (/docs) 적극 활용
4. 각 API마다 Postman으로 테스트

### 난이도 표시
- 🟢 기초: 오늘 배운 내용만
- 🟡 응용: 이전 내용 + 오늘 내용
- 🔴 도전: 창의적 사고 필요

### 주의사항

**1. Day 6-1교시 가상환경**
- 기초 과정에서 import는 배웠지만 가상환경은 안 배움
- 실무 맥락에서 pip install → import 흐름 체험

**2. JSON 복습**
- Day 5에서 배웠으니 Day 6-6교시는 웹 맥락만 추가
- 문법 재설명 최소화, 웹에서의 활용 중심

**3. SQL 범위 제한**
- 복잡한 JOIN, 서브쿼리는 제외
- 기본 CRUD (SELECT, INSERT, UPDATE, DELETE)만

**4. Day 10 프로젝트**
- 완성도보다 경험 중심
- 간단한 주제 선택 권장
- 6-8교시 총 150분 활용

**5. 에러 처리 강조**
- 실제로 에러를 발생시켜 보며 학습
- 422 Unprocessable Entity 이해

---

## 🔧 트러블슈팅 가이드

### 자주 발생하는 문제

**1. 가상환경 활성화 안 됨**
```bash
# Git Bash
source venv/Scripts/activate

# 확인
which python  # venv 경로가 나와야 함
```

**2. uvicorn 실행 안 됨**
```bash
# FastAPI, uvicorn 재설치
pip install --upgrade fastapi uvicorn
```

**3. 포트 이미 사용 중**
```bash
# 다른 포트 사용
uvicorn main:app --reload --port 8001
```

**4. 422 Unprocessable Entity**
- Pydantic 검증 실패
- /docs에서 자동 생성된 스키마 확인
- 타입 불일치 확인

**5. 404 Not Found**
- URL 경로 확인
- 함수 데코레이터 확인 (@app.get)
- 서버 재시작 (--reload 옵션 사용 권장)

**6. CORS 오류 (브라우저)**
```python
from fastapi.middleware.cors import CORSMiddleware

app.add_middleware(
    CORSMiddleware,
    allow_origins=["*"],
    allow_credentials=True,
    allow_methods=["*"],
    allow_headers=["*"],
)
```

---

## 📚 참고 자료

### 교재
- 처음 시작하는 FastAPI (빌 루바노빅)

### 온라인 리소스
- FastAPI 공식 문서: https://fastapi.tiangolo.com/
- Pydantic 공식 문서: https://docs.pydantic.dev/
- SQLite 튜토리얼: https://www.sqlitetutorial.net/
- Postman 학습: https://learning.postman.com/
- 공개 API (테스트용): https://jsonplaceholder.typicode.com/

### 추천 도구
- Postman: API 테스팅
- SQLite Browser: 데이터베이스 GUI
- Thunder Client: VS Code 확장 (Postman 대체)

---

## 🎓 평가 기준

### 출석 및 참여 (30%)
- 매일 출석
- 실습 참여도

### 실습 과제 (40%)
- Exercise 완성도
- 종합 Problem 해결

### 최종 프로젝트 (30%)
- API 설계 적절성
- 기능 구현 완성도
- 코드 품질
- 발표 및 시연

---

## 🎯 응용 과정 완료 후 체크리스트

### 학생이 할 수 있어야 하는 것:
- [ ] 웹 동작 원리 이해
- [ ] HTTP 메서드, 상태 코드 이해
- [ ] REST API 설계 원칙 적용
- [ ] FastAPI로 기본 API 작성
- [ ] 경로/쿼리 매개변수 활용
- [ ] Pydantic 모델 정의
- [ ] Request Body 처리
- [ ] SQLite 데이터베이스 연동
- [ ] CRUD API 완성
- [ ] Postman으로 API 테스트
- [ ] 에러 처리 (HTTPException)
- [ ] 자동 문서 활용

### 심화 과정 준비 상태:
- [ ] FastAPI 기본 익숙함
- [ ] 데이터베이스 연동 가능
- [ ] REST API 설계 이해
- [ ] Pydantic 모델 활용 가능

---

**최종 수정일**: 2026-01-29
**버전**: 3.0
**주요 변경 사항**:
- Day 6-1교시에 가상환경 + import 실무 추가
- Day 6-6교시 JSON을 복습 + 웹 맥락으로 변경
- Day 10 프로젝트 시간 유지 (6-8교시)
- 기초 과정 변경사항 반영 (JSON, import)
