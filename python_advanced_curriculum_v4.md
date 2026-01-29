# Python 심화 과정 커리큘럼 v4.0

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
- Exercise: 5-10분

**8교시 종합 실습 (50분)**
- 복습 퀴즈: 10분
- 🟢 기초 Problem: 15분
- 🟡 응용 Problem: 15-20분
- 🔴 도전 Problem: 5-10분

**복습 교시 (매일 1교시, 50분)**
- 퀴즈: 20분
- 실습 복습: 25분
- Q&A: 5분

**프로젝트 교시 (Day 15)**
- 구현: 1-6교시 (300분)
- 발표: 7-8교시 (100분)

---

## Day 11: 프로젝트 구조와 의존성 주입

### 1교시: 응용 과정 복습 + 심화 과정 오리엔테이션
- **퀴즈 (20분)**: FastAPI 기본, Pydantic, CRUD, REST API
- **심화 과정 소개 (15분)**: 로드맵, 최종 목표, 프로덕션 레벨 API
- **환경 체크 (10분)**: 가상환경, FastAPI, 이전 프로젝트 확인
- **Q&A (5분)**

### 2교시: 프로젝트 구조 설계 ⭐⭐⭐
- **개념 (12분)**: 계층 구조 (Web-Service-Data), 관심사의 분리, 확장 가능한 구조
- **Basic (22분)**: 디렉터리 구조, 파일 역할, __init__.py, 모듈 import 패턴
- **Practice (10분)**: 프로젝트 구조 만들기 (함께)
- **Exercise (6분)**: 자신의 프로젝트 구조 설계

### 3교시: 라우터 고급 분리 ⭐⭐
- **개념 (8분)**: 도메인별 라우터, tags/prefix 활용, 계층별 책임
- **Basic (20분)**: APIRouter 심화, include_router, 여러 라우터 조합, 라우터 간 의존성
- **Practice (15분)**: users, posts, comments 라우터 분리
- **Exercise (7분)**: 3개 이상 도메인 라우터 구성

### 4교시: 의존성 주입 개념 ⭐⭐⭐
- **개념 (15min)**: DI(Dependency Injection)란?, 왜 필요한가?, FastAPI의 Depends, 테스트 용이성
- **Basic (20분)**: 
  - 간단한 의존성
  - 함수를 의존성으로
  - 클래스를 의존성으로
  - 의존성 체인
- **Practice (10분)**: 설정 의존성, 로깅 의존성 만들기
- **Exercise (5분)**: 커스텀 의존성 작성

### 5교시: 데이터베이스 의존성 ⭐⭐⭐
- **개념 (12분)**: get_db() 패턴, 연결 관리, 자동 close, yield, 트랜잭션
- **Basic (20분)**: 
  - DB 연결 의존성
  - yield 사용
  - 에러 시 rollback
  - 실전 패턴
- **Practice (13분)**: get_db() 구현, 모든 엔드포인트에 적용
- **Exercise (5분)**: DB 의존성 테스트

### 6교시: 환경 변수 관리 + DI 추가 실습 ⭐⭐
- **개념 (7분)**: .env 파일, 환경별 설정 (dev/prod), 비밀 정보 관리
- **Basic (15분)**: 
  - python-dotenv
  - 설정 클래스
  - Pydantic Settings
  - 환경 변수 주입
- **Practice (12분)**: .env 파일 생성, Settings 클래스 작성
- **DI 추가 실습 (10분)**: 
  - Settings를 의존성으로 활용
  - 여러 의존성 조합 연습
- **Exercise (6분)**: 환경별 설정 분리

### 7교시: 계층별 코드 분리 기본 ⭐⭐⭐
- **개념 (10분)**: Web(라우터) / Service(비즈니스) / Data(DB) 계층, 각 계층의 역할
- **Basic (22분)**: 
  - 계층별 파일 구조
  - 함수 분리
  - 의존성 흐름
- **Practice (13분)**: 간단한 CRUD를 계층별로 리팩토링
- **Exercise (5분)**: 새 기능을 계층별로 구현

> **참고**: Day 12-1교시에서 계층 분리 심화 진행

### 8교시: Day 11 종합 실습
- **복습 퀴즈 (10분)**: 프로젝트 구조, DI, 계층 분리
- **🟢 기초 Problem (15분)**: 계층 구조로 TODO API 리팩토링
- **🟡 응용 Problem (20분)**: 완전한 3계층 구조 구축 + 의존성 활용
- **🔴 도전 Problem (5분)**: 의존성 체인 최적화

---

## Day 12: 인증 기초 - 패스워드와 JWT

### 1교시: Day 11 복습 + 계층 분리 심화
- **퀴즈 (15분)**: 프로젝트 구조, 의존성 주입
- **계층 분리 심화 (25분)**: 
  - 복잡한 비즈니스 로직 분리
  - Service 계층 패턴
  - 실습: 게시판 API를 완전한 3계층으로
- **Q&A (10분)**

### 2교시: 인증과 인가 개념 ⭐⭐⭐
- **개념 (15분)**: Authentication vs Authorization, 세션 vs 토큰, JWT 소개, 보안의 중요성
- **Basic (20분)**: 
  - 인증 흐름 도식화
  - 토큰 기반 인증
  - JWT 구조 (Header/Payload/Signature)
- **Practice (10분)**: JWT 디코딩 실습 (jwt.io)
- **Exercise (5분)**: 인증 시나리오 분석

### 3교시: 패스워드 해싱 + JWT 기초 ⭐⭐⭐
- **개념 (10분)**: 
  - 평문 저장의 위험성
  - 해시 함수, Salt
  - JWT 상세 구조, 클레임, 만료 시간
- **Basic (22분)**: 
  - passlib 설치 및 사용
  - 해시 생성, 검증
  - python-jose 설치
  - SECRET_KEY, 알고리즘
- **Practice (13분)**: 
  - 패스워드 해싱 함수 구현
  - JWT 기본 개념 실습
- **Exercise (5분)**: 해싱 + JWT 도구 함수 작성

### 4교시: JWT 생성과 검증 통합 ⭐⭐⭐
- **개념 (8분)**: 토큰 생성 → 검증 전체 흐름
- **Basic (25분)**: 
  - create_access_token() 함수
  - 페이로드 구성
  - verify_token() 함수
  - jwt.decode()
  - 예외 처리 (ExpiredSignatureError)
- **Practice (12분)**: 토큰 생성 → 검증 전체 흐름 구현
- **Exercise (5분)**: 토큰 검증 테스트, 커스텀 클레임

### 5교시: JWT 검증 심화 + 보안 ⭐⭐
- **개념 (8min)**: 토큰 탈취 방지, 만료 시간 설정, 보안 고려사항
- **Basic (20분)**: 
  - 서명 검증
  - 만료 확인
  - 토큰에서 사용자 정보 추출
  - 보안 패턴
- **Practice (15분)**: 
  - 안전한 토큰 검증 구현
  - 에러 처리 강화
- **Exercise (7분)**: 토큰 보안 테스트

### 6교시: 회원가입 구현 ⭐⭐
- **개념 (7분)**: 회원가입 플로우, 사용자 모델, 중복 체크
- **Basic (20분)**: 
  - User 모델 (Pydantic)
  - DB 테이블
  - 중복 이메일 체크
  - 해싱 적용
- **Practice (15분)**: 회원가입 API 완성
- **Exercise (8min)**: 유효성 검증 강화 (이메일 형식, 비밀번호 강도)

### 7교시: 로그인 구현 ⭐⭐⭐
- **개념 (8분)**: 로그인 플로우, 사용자 검증, 토큰 발급
- **Basic (22분)**: 
  - 로그인 엔드포인트
  - 이메일/패스워드 검증
  - 토큰 생성 및 반환
  - 에러 처리 (401)
- **Practice (13분)**: 로그인 API 완성
- **Exercise (7분)**: Postman으로 전체 흐름 테스트 (회원가입 → 로그인 → 토큰 확인)

### 8교시: Day 12 종합 실습
- **복습 퀴즈 (10분)**: 해싱, JWT, 인증
- **🟢 기초 Problem (15분)**: 간단한 인증 시스템 구축
- **🟡 응용 Problem (20분)**: 회원가입 + 로그인 + 토큰 검증 완성
- **🔴 도전 Problem (5분)**: 토큰 갱신(Refresh Token) 로직

---

## Day 13: OAuth2와 권한 관리

### 1교시: Day 12 복습
- **퀴즈 (20분)**: 패스워드 해싱, JWT, 인증
- **실습 복습 (25분)**: 로그인 재구현, 토큰 검증
- **Q&A (5분)**

### 2교시: OAuth2 개념 ⭐⭐⭐
- **개념 (15분)**: OAuth2란?, 흐름(Flow), Password Flow, FastAPI의 OAuth2PasswordBearer
- **Basic (20분)**: 
  - OAuth2 구조
  - tokenUrl
  - Bearer 토큰
  - Authorization 헤더
- **Practice (10분)**: OAuth2PasswordBearer 설정
- **Exercise (5분)**: OAuth2 플로우 이해 확인

### 3교시: OAuth2PasswordBearer 구현 ⭐⭐⭐
- **개념 (8분)**: OAuth2PasswordBearer 사용법, 의존성으로 활용
- **Basic (22분)**: 
  - OAuth2PasswordBearer 인스턴스 생성
  - 토큰 추출
  - 자동 문서 연동 (자물쇠 아이콘)
- **Practice (13분)**: 기존 인증에 OAuth2 적용
- **Exercise (7분)**: 토큰 추출 테스트

### 4교시: 현재 사용자 가져오기 ⭐⭐⭐
- **개념 (10분)**: get_current_user 패턴, 의존성 체인, 사용자 정보 활용
- **Basic (22분)**: 
  - get_current_user() 함수
  - 토큰 검증 + DB 조회
  - HTTPException 처리
  - 의존성으로 주입
- **Practice (10분)**: 현재 사용자 의존성 구현
- **Exercise (8분)**: 프로필 API에 적용

### 5교시: 보호된 엔드포인트 ⭐⭐⭐
- **개념 (8min)**: 인증 필요 API, Depends로 보호, 로그인하지 않은 사용자 차단
- **Basic (20분)**: 
  - 의존성으로 사용자 요구
  - 자동 문서의 자물쇠 아이콘
  - 401 Unauthorized
  - 실전 패턴
- **Practice (15분)**: 
  - 마이페이지 API
  - 게시글 작성 API
  - 댓글 작성 API
- **Exercise (7분)**: 전체 API에 인증 적용

### 6교시: 인가 (Authorization) ⭐⭐⭐
- **개념 (10분)**: 인증 vs 인가, 역할(Role), RBAC, 권한 체크
- **Basic (22분)**: 
  - User 모델에 role 추가
  - 권한 체크 의존성
  - admin만 접근 가능한 API
- **Practice (13분)**: 관리자 권한 체크 구현
- **Exercise (5분)**: 여러 역할 구현 (user, admin, moderator)

### 7교시: CORS 설정 ⭐⭐
- **개념 (10분)**: CORS란?, Origin, Preflight, 왜 필요한가?
- **Basic (22분)**: 
  - CORSMiddleware
  - 허용 도메인
  - 허용 메서드
  - 실전 설정
- **Practice (13분)**: CORS 설정, 프론트엔드 연동 준비
- **Exercise (5min)**: 환경별 CORS 설정

### 8교시: Day 13 종합 실습
- **복습 퀴즈 (10분)**: OAuth2, 인가, CORS
- **🟢 기초 Problem (15분)**: OAuth2 인증 적용
- **🟡 응용 Problem (20분)**: 역할 기반 권한 시스템 (user/admin)
- **🔴 도전 Problem (5분)**: 복잡한 권한 로직 (리소스 소유권 체크)

---

## Day 14: 비동기 프로그래밍과 고급 기능

### 1교시: Day 13 복습
- **퀴즈 (20분)**: OAuth2, 인가, CORS
- **실습 복습 (25분)**: 권한 체크 재구현
- **Q&A (5분)**

### 2교시: 비동기 개념과 필요성 ⭐⭐⭐
- **개념 (15분)**: 
  - 블로킹 vs 논블로킹
  - 동시성
  - I/O 대기 시간
  - FastAPI와 비동기
  - **언제 사용하나?** (중요!)
- **Basic (22분)**: 
  - 동기 코드의 문제점
  - 비동기의 장점
  - 성능 비교 시뮬레이션
- **Practice (8분)**: 시뮬레이션 (동기 vs 비동기 시간 차이)
- **Exercise (5분)**: 비동기가 필요한 상황 판단

### 3교시: async/await 기본 ⭐⭐⭐
- **개념 (10min)**: async def, await 키워드, asyncio 기본
- **Basic (22분)**: 
  - 비동기 함수 정의
  - await로 호출
  - asyncio.sleep()
  - 여러 작업 동시 실행 (간단히)
- **Practice (13분)**: 간단한 비동기 함수 작성
- **Exercise (5분)**: 비동기 패턴 연습

### 4교시: httpx로 외부 API 호출 ⭐⭐
- **개념 (8분)**: httpx, 비동기 HTTP 클라이언트, 실전 활용
- **Basic (22분)**: 
  - httpx 설치
  - AsyncClient
  - 외부 API 호출
  - 여러 요청 동시 처리
- **Practice (13분)**: 비동기 API 호출 구현
- **Exercise (7분)**: 여러 외부 API 동시 호출

### 5교시: 백그라운드 태스크 ⭐⭐
- **개념 (10분)**: BackgroundTasks, 비동기 작업 처리, 사용 사례
- **Basic (20분)**: 
  - BackgroundTasks 사용
  - 이메일 전송 예시
  - 로그 기록
  - 파일 처리
- **Practice (15분)**: 백그라운드 작업 구현
- **Exercise (5분)**: 이미지 처리 백그라운드 작업

### 6교시: 파일 업로드 ⭐⭐
- **개념 (8min)**: UploadFile, 파일 저장, 보안 고려
- **Basic (22분)**: 
  - File(), UploadFile
  - 파일 저장
  - 파일 크기 제한
  - 파일 타입 검증
- **Practice (13분)**: 이미지 업로드 API
- **Exercise (7분)**: 프로필 사진 업로드

### 7교시: 파일 다운로드 ⭐⭐
- **개념 (7min)**: FileResponse, 파일 제공, Content-Disposition
- **Basic (20분)**: 
  - FileResponse 사용
  - 파일 다운로드
  - 미디어 타입 설정
- **Practice (15분)**: 파일 다운로드 API
- **Exercise (8분)**: 업로드 + 다운로드 통합

### 8교시: Day 14 종합 실습
- **복습 퀴즈 (10분)**: 비동기, 백그라운드 태스크, 파일
- **🟢 기초 Problem (15분)**: 비동기 API 만들기 (httpx)
- **🟡 응용 Problem (20분)**: 파일 업로드 + 백그라운드 처리 (썸네일 생성 등)
- **🔴 도전 Problem (5분)**: 여러 외부 API 동시 호출 + 결과 통합

---

## Day 15: 최종 프로젝트

### 1교시: Day 14 복습 + 프로젝트 킥오프
- **퀴즈 (15분)**: 비동기, 파일, 전체 복습
- **프로젝트 안내 (20분)**: 
  - 요구사항
  - 평가 기준
  - 시간 배분
  - 예시 프로젝트 소개
- **팀/주제 선정 (10분)**: 개인 권장, 주제 결정
- **Q&A (5분)**

### 2교시: 프로젝트 기획 및 설계
- **요구사항 분석 (20분)**: 
  - 기능 목록 작성
  - 우선순위 결정 (MVP 중심)
- **API 설계 (20min)**: 
  - 엔드포인트 설계
  - Request/Response 모델
- **DB 스키마 설계 (10분)**: 테이블 구조, 관계 설정

### 3교시: 프로젝트 구현 (1) - 기본 구조
- **프로젝트 초기화 (15분)**: 
  - 디렉터리 구조 (3계층)
  - 가상환경
  - 설정 파일 (.env)
- **DB 모델 작성 (20분)**: 테이블 생성, 초기 데이터
- **기본 CRUD (15분)**: 핵심 엔드포인트 구현

### 4교시: 프로젝트 구현 (2) - 인증 적용
- **사용자 모델 (15분)**: User 테이블, 패스워드 해싱
- **인증 구현 (25분)**: 
  - 회원가입
  - 로그인
  - JWT
- **보호 적용 (10분)**: 인증 필요 API에 적용

### 5교시: 프로젝트 구현 (3) - 핵심 기능
- **핵심 기능 구현 (35분)**: 
  - 주요 비즈니스 로직
  - Service 계층 활용
  - 검증 강화
- **에러 처리 (15분)**: 
  - HTTPException
  - 일관된 에러 응답

### 6교시: 프로젝트 구현 (4) - 추가 기능 및 마무리
- **추가 기능 (25분)**: 
  - 선택 사항 (파일 업로드, 검색, 필터링 등)
  - 페이지네이션
- **코드 정리 (15분)**: 
  - 리팩토링
  - 주석 추가
  - 코드 품질 개선
- **테스트 및 문서화 (10분)**: 
  - Postman 테스트
  - README 작성

### 7교시: 프로젝트 발표 (1) ⭐⭐⭐
- **발표 준비 (10분)**: 시연 순서, 포인트 정리
- **발표 1-3팀 (40분)**: 각 팀 12-13분
  - 시연: 5-6분
  - 설명: 4-5분
  - 질의응답: 3-4분

### 8교시: 프로젝트 발표 (2) + 마무리 ⭐⭐⭐
- **발표 4-6팀 (40분)**: 각 팀 12-13분
  - 시연: 5-6분
  - 설명: 4-5분
  - 질의응답: 3-4분
- **전체 회고 (10분)**: 
  - 베스트 프로젝트 선정
  - 배운 점 공유
  - 아쉬운 점 정리
  - 향후 학습 방향

> **참고**: 수료식은 별도 진행 또는 생략 (프로젝트 중심)

---

## 📌 핵심 학습 목표 (프로덕션 레벨)

### 최우선 항목 ⭐⭐⭐
1. **프로젝트 구조**: 계층 분리 (Web-Service-Data), 확장 가능한 구조
2. **의존성 주입**: FastAPI Depends 마스터
3. **JWT 인증**: 회원가입, 로그인, 토큰 검증 전체 흐름
4. **OAuth2 패턴**: 표준 인증 구현
5. **권한 관리**: 역할 기반 접근 제어 (RBAC)
6. **환경 변수**: 설정 관리, 보안

### 중요 항목 ⭐⭐
1. 비동기 프로그래밍 기본 (개념 이해)
2. CORS 설정
3. 파일 업로드/다운로드
4. 백그라운드 태스크

### 기본 항목 ⭐
1. httpx 활용
2. 성능 최적화 개념

---

## 💡 교육 운영 팁

### 준비 사항
- [ ] passlib, python-jose 설치 가이드
- [ ] python-dotenv 설치 가이드
- [ ] httpx 설치 가이드 (선택)
- [ ] 각 일차별 PPT 슬라이드
- [ ] 각 일차별 코드 예제 (.py 파일)
- [ ] 전체 정답 코드
- [ ] 프로젝트 예시 3가지 (블로그, TODO, 쇼핑몰)
- [ ] 트러블슈팅 FAQ

### 권장 프로젝트 구조
```
my-fastapi-project/
├── app/
│   ├── __init__.py
│   ├── main.py              # FastAPI 앱
│   ├── config.py            # 설정
│   ├── dependencies.py      # 공통 의존성
│   ├── routers/             # 라우터 (Web 계층)
│   │   ├── __init__.py
│   │   ├── users.py
│   │   └── posts.py
│   ├── services/            # 비즈니스 로직 (Service 계층)
│   │   ├── __init__.py
│   │   ├── user_service.py
│   │   └── post_service.py
│   ├── database/            # DB 관련 (Data 계층)
│   │   ├── __init__.py
│   │   ├── connection.py
│   │   └── models.py
│   ├── schemas/             # Pydantic 모델
│   │   ├── __init__.py
│   │   ├── user.py
│   │   └── post.py
│   └── utils/               # 유틸리티
│       ├── __init__.py
│       ├── auth.py
│       └── security.py
├── .env                     # 환경 변수
├── .gitignore
├── requirements.txt
└── README.md
```

### 필수 패키지 설치
```bash
# 기본
pip install fastapi uvicorn

# 인증
pip install passlib[bcrypt] python-jose[cryptography] python-multipart

# 환경 변수
pip install python-dotenv

# 비동기 (선택)
pip install httpx aiofiles

# requirements.txt 생성
pip freeze > requirements.txt
```

### .env 파일 예시
```
# 애플리케이션
APP_NAME=My FastAPI App
DEBUG=True

# 데이터베이스
DATABASE_URL=sqlite:///./app.db

# JWT
SECRET_KEY=your-secret-key-here-change-in-production
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30

# CORS
ALLOWED_ORIGINS=http://localhost:3000,http://localhost:8080
```

### JWT Secret Key 생성
```python
# Python으로 생성
import secrets
print(secrets.token_urlsafe(32))
```

### 난이도 표시
- 🟢 기초: 오늘 배운 내용만
- 🟡 응용: 이전 내용 + 오늘 내용
- 🔴 도전: 창의적 사고 필요

### 주의사항

**1. 인증 파트 (Day 12-13)**
- 개념이 어려우니 천천히
- 토큰을 실제로 복사해서 테스트
- Postman에서 Authorization 설정 방법 명확히
- Day 12에서 통합 교시로 효율적 학습

**2. 비동기 파트 (Day 14)**
- **깊이보다 "왜 필요한가?" 중심** (v4 강조)
- 성능 차이를 직접 체험하도록
- 모든 것을 비동기로 바꿀 필요는 없음
- 3교시로 축소하여 핵심만

**3. 프로젝트 (Day 15)**
- 완성도보다 학습 경험 중심
- 너무 복잡한 기능은 피하기
- 시간 관리 철저히
- 발표 시간 균등 배분 (각 12-13분)

**4. 계층 분리**
- Day 11에서 기본, Day 12-1교시에서 심화
- 점진적 학습으로 소화 가능

---

## 🔧 트러블슈팅 가이드

### 자주 발생하는 문제

**1. JWT 토큰 관련**
```python
# ExpiredSignatureError
# → 토큰 만료 시간 확인

# JWTError
# → SECRET_KEY 일치 확인
# → 토큰 형식 확인 (Bearer 포함 여부)
```

**2. 패스워드 해싱**
```bash
# passlib 설치 오류
pip install passlib[bcrypt]

# bcrypt 관련 오류 (Windows)
# → pip install bcrypt 먼저 설치
```

**3. OAuth2 인증**
```python
# 401 Unauthorized
# → Authorization 헤더 확인
# → Bearer 토큰 형식 확인

# Postman 설정
# → Authorization 탭
# → Type: Bearer Token
# → Token: (로그인에서 받은 토큰)
```

**4. CORS 오류**
```python
# 브라우저에서 차단
# → CORSMiddleware 추가
# → allow_origins에 프론트엔드 URL 추가

from fastapi.middleware.cors import CORSMiddleware

app.add_middleware(
    CORSMiddleware,
    allow_origins=["http://localhost:3000"],
    allow_credentials=True,
    allow_methods=["*"],
    allow_headers=["*"],
)
```

**5. 비동기 관련**
```python
# "coroutine was never awaited"
# → async 함수는 await으로 호출

# "cannot use sync function in async context"
# → 비동기 컨텍스트에서는 비동기 함수 사용
```

**6. httpx 설치**
```bash
# httpx 설치
pip install httpx

# 설치 확인
pip list | grep httpx
```

---

## 📚 참고 자료

### 교재
- 처음 시작하는 FastAPI (빌 루바노빅)

### 공식 문서
- FastAPI: https://fastapi.tiangolo.com/
- Pydantic: https://docs.pydantic.dev/
- JWT: https://jwt.io/
- OAuth 2.0: https://oauth.net/2/
- passlib: https://passlib.readthedocs.io/

### 추천 도구
- Postman: API 테스팅
- JWT.io: JWT 디코더
- SQLite Browser: 데이터베이스 GUI

### 추가 학습 자료
- FastAPI 공식 튜토리얼
- Real Python - FastAPI 시리즈
- FastAPI GitHub Examples

---

## 🎓 평가 기준

### 출석 및 참여 (20%)
- 매일 출석
- 실습 참여도

### 실습 과제 (30%)
- Exercise 완성도
- 종합 Problem 해결

### 최종 프로젝트 (50%)
- **기획 (10%)**: 요구사항 분석, API 설계
- **구현 (25%)**: 기능 완성도, 코드 품질
- **인증/권한 (10%)**: JWT, OAuth2 적용
- **발표 (5%)**: 시연, 설명

---

## 🎯 프로젝트 평가 체크리스트

### 필수 요구사항 (70%)
- [ ] 계층 구조 (Web-Service-Data)
- [ ] 의존성 주입 활용
- [ ] 회원가입/로그인 (JWT)
- [ ] 인증이 필요한 엔드포인트
- [ ] CRUD 기본 기능
- [ ] 에러 처리
- [ ] .env 환경 변수 관리

### 추가 점수 (30%)
- [ ] 권한 관리 (역할 기반)
- [ ] 비동기 활용
- [ ] 파일 업로드
- [ ] CORS 설정
- [ ] 페이지네이션
- [ ] 코드 품질 (주석, 구조)
- [ ] README 문서화

---

## 🏆 수료 후 학습 방향

### 즉시 적용 가능
1. **개인 프로젝트**: 배운 내용으로 실제 서비스 구축
2. **오픈소스 기여**: FastAPI 관련 프로젝트 참여
3. **포트폴리오**: GitHub에 프로젝트 공개

### 추가 학습 권장
1. **테스팅**: pytest, coverage
2. **배포**: Docker, AWS, Heroku
3. **데이터베이스**: PostgreSQL, MongoDB
4. **ORM**: SQLAlchemy, Tortoise ORM
5. **프론트엔드 연동**: React, Vue.js
6. **고급 주제**: 
   - WebSocket
   - GraphQL
   - 마이크로서비스
   - 캐싱 (Redis)
   - 메시지 큐 (RabbitMQ, Celery)

---

## 📝 v3에서 v4 주요 변경사항

### Day 11 개선
- **6교시**: 환경 변수(30분) + DI 추가 실습(20분) 통합
- **7교시**: 계층 분리 "기본"으로 변경
- **Day 12-1교시**: 계층 분리 "심화" 추가

### Day 12 통합 개선 ⭐
- **3교시**: 패스워드 해싱 + JWT 기초 통합
- **4-5교시**: JWT 생성/검증 통합 → 심화
- **6-7교시**: 회원가입 + 로그인 (기존과 동일하지만 흐름 개선)

### Day 14 비동기 축소 ⭐
- **2-3교시**: 비동기 개념 + async/await (기존 4교시 → 2교시)
- **4교시**: httpx 실전 (기존 비동기 라이브러리)
- **5교시**: 백그라운드 태스크 (기존과 동일)
- **6-7교시**: 파일 업로드/다운로드 분리
- **비동기 개념 정리 교시 제거**: 중복 제거

### Day 15 발표 개선 ⭐
- **7-8교시**: 발표 시간 균등 배분 (각 팀 12-13분)
- **수료식**: 별도 또는 생략 (프로젝트 중심)

### 전체 흐름 개선
1. DI 내용 분산 (Day 11-12)
2. 인증 통합 교시로 효율화
3. 비동기 핵심만 (깊이 축소)
4. 발표 시간 공평하게

---

**최종 수정일**: 2026-01-29
**버전**: 4.0
**작성자**: FastAPI 교육 커리큘럼 팀
**이전 과정**: Python 응용 과정 v4.0 (Day 6-10)
**수료 후**: 프로덕션 레벨 FastAPI 개발자
