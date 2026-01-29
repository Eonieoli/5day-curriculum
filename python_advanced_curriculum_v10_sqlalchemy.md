# Python 심화 과정 커리큘럼 v10 (SQLAlchemy)

## 📋 과정 개요

- **과정명**: Python 심화 과정 (SQLAlchemy)
- **목표**: 프로덕션 수준의 FastAPI 백엔드 서버 구축 (SQLAlchemy ORM 사용)
- **기간**: 5일 (Day 11 ~ Day 15)
- **일일 시간**: 8교시 (명목상 50분 × 8 = 400분, 실제 약 7시간)
- **총 시간**: 약 35시간
- **선수 과정**: Python 기초 과정 (Day 1-5), Python 응용 과정 (Day 6-10, SQLAlchemy)
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

**복습 교시 (매일 1교시, 50분)**

- 복습 퀴즈: 10분 (간소화!)
- 핵심 복습: 15분 (전날 가장 중요한 것만!)
- 새 내용: 25분 (바로 진도!)

**프로젝트 교시 (Day 15)**

- 추가 주제: 2-4교시 (150분)
- 프로젝트: 5-8교시 (200분)

---

## Day 11: 프로젝트 구조와 의존성 주입

### 1교시: 응용 과정 복습 + 프로젝트 구조 시작

- **복습 퀴즈 (10분)**: FastAPI 기본, Pydantic, SQLAlchemy, REST API
- **핵심 복습 (15분)**:
  - SQLAlchemy 모델 복습
  - Session 관리 복습
  - relationship 복습
  - 간단한 Q&A
- **프로젝트 구조 시작 (25분)**:
  - 심화 과정 소개 (5분):
    - 로드맵
    - 최종 목표 (프로덕션 레벨 API)
    - 5일 계획
  - 환경 체크 (5분):
    - 가상환경 확인
    - FastAPI, SQLAlchemy 확인
  - 개념 (15분):
    - 계층 구조 (Web-Service-Data)
    - 관심사의 분리
    - 확장 가능한 구조
    - 왜 필요한가?

### 2교시: 프로젝트 구조 설계 ⭐⭐⭐

- **Basic (25분)**:
  - 디렉터리 구조
  ```
  project/
  ├── app/
  │   ├── __init__.py
  │   ├── main.py          # FastAPI 앱
  │   ├── database.py      # DB 설정, Session
  │   ├── models/          # SQLAlchemy 모델
  │   │   ├── __init__.py
  │   │   ├── user.py
  │   │   └── post.py
  │   ├── schemas/         # Pydantic 스키마
  │   │   ├── __init__.py
  │   │   ├── user.py
  │   │   └── post.py
  │   ├── routers/         # API 엔드포인트
  │   │   ├── __init__.py
  │   │   ├── users.py
  │   │   └── posts.py
  │   └── services/        # 비즈니스 로직
  │       ├── __init__.py
  │       ├── user_service.py
  │       └── post_service.py
  ├── .env
  ├── .gitignore
  └── requirements.txt
  ```
  - 파일 역할
  - **__init__.py
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
- **Basic (25분)**:
  - python-dotenv (5분)
  - 설정 클래스 (5분)
  - Pydantic Settings (5min)
  - 환경 변수 주입 (5min)
  - **환경 변수 검증** (필수 값 체크) (5min)
- **보안 경고 (5분)**:
  - **🚨 .gitignore에 .env 필수!**
    ```
    # .gitignore
    .env
    __pycache__/
    *.pyc
    *.db
    ```
  - **.env.example 파일 만들기**:
    ```
    # .env.example (실제 값 없이 템플릿만)
    DATABASE_URL=sqlite:///./app.db
    SECRET_KEY=your_secret_key_here
    ```
  - **절대 .env를 커밋하지 말 것!**
  - **실제 사례 경고**:
    - AWS 키 유출 → 수백만 원 청구
    - DB 비밀번호 유출 → 해킹
    - GitHub에서 자동 스캔으로 즉시 발견됨
- **Practice (5min)**:
  - .env 파일 생성
  - .gitignore 추가
  - .env.example 작성
- **Exercise (5min)**:
  - 환경별 설정 분리

### 6교시: 데이터베이스 의존성 (SQLAlchemy) ⭐⭐⭐

- **개념 (12min)**:
  - get_db() 패턴 (SQLAlchemy 버전)
  - Session 관리
  - 자동 close
  - yield의 중요성
  - 트랜잭션 관리

- **Basic (20min)**:
  ```python
  # app/database.py
  from sqlalchemy import create_engine
  from sqlalchemy.ext.declarative import declarative_base
  from sqlalchemy.orm import sessionmaker, Session
  from typing import Generator
  
  SQLALCHEMY_DATABASE_URL = "sqlite:///./app.db"
  
  engine = create_engine(
      SQLALCHEMY_DATABASE_URL,
      connect_args={"check_same_thread": False}  # SQLite only
  )
  
  SessionLocal = sessionmaker(
      autocommit=False,
      autoflush=False,
      bind=engine
  )
  
  Base = declarative_base()
  
  # 의존성 함수
  def get_db() -> Generator[Session, None, None]:
      db = SessionLocal()
      try:
          yield db
      finally:
          db.close()
  
  # 엔드포인트에서 사용
  from fastapi import Depends
  
  @app.get("/users/{user_id}")
  def get_user(
      user_id: int,
      db: Session = Depends(get_db)  # 자동 주입!
  ):
      user = db.query(User).filter(User.id == user_id).first()
      if not user:
          raise HTTPException(status_code=404, detail="User not found")
      return user
  ```

- **Practice (10min)**:
  - get_db() 구현
  - 엔드포인트에 적용
  
- **Exercise (8min)**:
  - DB 의존성 테스트

### 7교시: 계층 분리 완전 정복 (SQLAlchemy) ⭐⭐⭐

- **개념 (10min)**:
  - Web(라우터) / Service(비즈니스) / Data(SQLAlchemy 모델) 계층
  - 각 계층의 역할과 책임
  - 실전 프로젝트 구조

- **기본 분리 (15min)**:
  - Basic (10min):
    ```python
    # app/models/user.py (Data 계층)
    from sqlalchemy import Column, Integer, String
    from app.database import Base
    
    class User(Base):
        __tablename__ = "users"
        
        id = Column(Integer, primary_key=True, index=True)
        email = Column(String, unique=True, index=True)
        hashed_password = Column(String)
    
    # app/schemas/user.py (Pydantic)
    from pydantic import BaseModel
    
    class UserCreate(BaseModel):
        email: str
        password: str
    
    class UserResponse(BaseModel):
        id: int
        email: str
        
        class Config:
            from_attributes = True  # SQLAlchemy 모델 변환
    
    # app/services/user_service.py (Service 계층)
    from sqlalchemy.orm import Session
    from app.models.user import User
    from app.schemas.user import UserCreate
    
    def create_user(db: Session, user_data: UserCreate) -> User:
        # 비즈니스 로직
        db_user = User(
            email=user_data.email,
            hashed_password=hash_password(user_data.password)
        )
        db.add(db_user)
        db.commit()
        db.refresh(db_user)
        return db_user
    
    def get_user_by_email(db: Session, email: str) -> User:
        return db.query(User).filter(User.email == email).first()
    
    # app/routers/users.py (Web 계층)
    from fastapi import APIRouter, Depends
    from sqlalchemy.orm import Session
    from app.database import get_db
    from app.schemas.user import UserCreate, UserResponse
    from app.services import user_service
    
    router = APIRouter(prefix="/users", tags=["users"])
    
    @router.post("/", response_model=UserResponse)
    def create_user_endpoint(
        user: UserCreate,
        db: Session = Depends(get_db)
    ):
        # 라우터는 요청/응답만 처리
        return user_service.create_user(db, user)
    ```
  - Practice (5min): 간단한 CRUD를 계층별로 리팩토링

- **심화 분리 (15min)**:
  - Basic (10min):
    ```python
    # 복잡한 비즈니스 로직 예시
    # app/services/post_service.py
    from sqlalchemy.orm import Session
    from app.models.post import Post
    from app.models.user import User
    
    def create_post_with_validation(
        db: Session,
        title: str,
        content: str,
        user_id: int
    ) -> Post:
        # 1. 사용자 확인 (비즈니스 로직)
        user = db.query(User).filter(User.id == user_id).first()
        if not user:
            raise ValueError("User not found")
        
        # 2. 제목 중복 확인
        existing = db.query(Post).filter(
            Post.title == title,
            Post.user_id == user_id
        ).first()
        if existing:
            raise ValueError("Duplicate title")
        
        # 3. 생성 (트랜잭션)
        try:
            post = Post(title=title, content=content, user_id=user_id)
            db.add(post)
            db.commit()
            db.refresh(post)
            return post
        except Exception as e:
            db.rollback()
            raise
    
    # 에러 처리 계층별 전략
    # Service: ValueError (비즈니스 로직 에러)
    # Router: HTTPException (HTTP 에러)
    
    # app/routers/posts.py
    @router.post("/")
    def create_post(
        title: str,
        content: str,
        user_id: int,
        db: Session = Depends(get_db)
    ):
        try:
            return post_service.create_post_with_validation(
                db, title, content, user_id
            )
        except ValueError as e:
            raise HTTPException(status_code=400, detail=str(e))
    ```
  - Practice (5min): 게시판 API를 완전한 3계층으로

- **실습 (10min)**:
  - Exercise: 새 기능을 계층별로 구현

### 8교시: Day 11 종합 실습

- **복습 퀴즈 (10min)**: 프로젝트 구조, DI, 계층 분리
- **🟢 기초 Problem (15min)**: 계층 구조로 TODO API 리팩토링
- **🟡 응용 Problem (15min)**: 완전한 3계층 구조 구축 + 의존성 활용
- **🔴 도전 Problem (10min)**: 의존성 체인 최적화

---

## Day 12: 인증 기초 - 패스워드와 JWT

### 1교시: Day 11 복습 + 인증 개념

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

### 6교시: 회원가입 구현 (SQLAlchemy) ⭐⭐

- **개념 (7min)**:
  - 회원가입 플로우
  - User 모델 (SQLAlchemy)
  - 중복 체크
- **Basic (20min)**:
  ```python
  # app/models/user.py
  from sqlalchemy import Column, Integer, String
  from app.database import Base
  
  class User(Base):
      __tablename__ = "users"
      
      id = Column(Integer, primary_key=True, index=True)
      email = Column(String, unique=True, index=True)
      hashed_password = Column(String)
  
  # app/services/auth_service.py
  from sqlalchemy.orm import Session
  from app.models.user import User
  from passlib.context import CryptContext
  
  pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")
  
  def create_user(db: Session, email: str, password: str):
      # 중복 체크
      existing = db.query(User).filter(User.email == email).first()
      if existing:
          raise ValueError("Email already registered")
      
      # 해싱 적용
      hashed = pwd_context.hash(password)
      
      user = User(email=email, hashed_password=hashed)
      db.add(user)
      db.commit()
      db.refresh(user)
      return user
  ```
- **Practice (13min)**:
  - 회원가입 API 완성
- **Exercise (10min)**:
  - 유효성 검증 강화

### 7교시: 로그인 구현 (SQLAlchemy) ⭐⭐⭐

- **개념 (8min)**:
  - 로그인 플로우
  - 사용자 검증
  - 토큰 발급
- **Basic (22min)**:
  ```python
  # app/services/auth_service.py
  def verify_password(plain: str, hashed: str) -> bool:
      return pwd_context.verify(plain, hashed)
  
  def authenticate_user(db: Session, email: str, password: str):
      # 이메일로 사용자 조회 (SQLAlchemy)
      user = db.query(User).filter(User.email == email).first()
      if not user:
          return None
      
      # 패스워드 검증
      if not verify_password(password, user.hashed_password):
          return None
      
      return user
  
  # app/routers/auth.py
  from app.services.auth_service import authenticate_user, create_access_token
  
  @router.post("/login")
  def login(email: str, password: str, db: Session = Depends(get_db)):
      user = authenticate_user(db, email, password)
      if not user:
          raise HTTPException(status_code=401, detail="Invalid credentials")
      
      # 토큰 생성
      token = create_access_token(data={"sub": user.email})
      return {"access_token": token, "token_type": "bearer"}
  ```
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

### 1교시: Day 12 복습 + OAuth2 시작

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

### 4교시: 현재 사용자 + 전역 에러 핸들러 ⭐⭐⭐

- **get_current_user (30min)**:
  - 개념 (7min):
    - get_current_user 패턴
    - 의존성 체인
    - 사용자 정보 활용
  - Basic (15min):
    ```python
    # app/dependencies/auth.py
    from fastapi import Depends, HTTPException, status
    from fastapi.security import OAuth2PasswordBearer
    from jose import JWTError, jwt
    from sqlalchemy.orm import Session
    from app.database import get_db
    from app.models.user import User
    
    oauth2_scheme = OAuth2PasswordBearer(tokenUrl="/auth/login")
    
    def get_current_user(
        token: str = Depends(oauth2_scheme),
        db: Session = Depends(get_db)
    ) -> User:
        try:
            # 토큰 검증
            payload = jwt.decode(token, SECRET_KEY, algorithms=[ALGORITHM])
            email: str = payload.get("sub")
            if email is None:
                raise HTTPException(
                    status_code=status.HTTP_401_UNAUTHORIZED,
                    detail="Invalid token"
                )
        except JWTError:
            raise HTTPException(
                status_code=status.HTTP_401_UNAUTHORIZED,
                detail="Invalid token"
            )
        
        # DB에서 사용자 조회 (SQLAlchemy)
        user = db.query(User).filter(User.email == email).first()
        if user is None:
            raise HTTPException(
                status_code=status.HTTP_401_UNAUTHORIZED,
                detail="User not found"
            )
        
        return user
    ```
  - Practice (5min): 현재 사용자 의존성 구현
  - Exercise (3min): 프로필 API에 적용

- **전역 에러 핸들러 (20min)**:
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
  ```python
  # app/models/user.py
  from sqlalchemy import Column, String, Enum
  import enum
  
  class UserRole(str, enum.Enum):
      USER = "user"
      ADMIN = "admin"
  
  class User(Base):
      __tablename__ = "users"
      
      id = Column(Integer, primary_key=True, index=True)
      email = Column(String, unique=True, index=True)
      hashed_password = Column(String)
      role = Column(String, default=UserRole.USER)
  
  # app/dependencies/auth.py
  def get_current_admin_user(
      current_user: User = Depends(get_current_user)
  ) -> User:
      if current_user.role != UserRole.ADMIN:
          raise HTTPException(
              status_code=status.HTTP_403_FORBIDDEN,
              detail="Not enough permissions"
          )
      return current_user
  
  # app/routers/admin.py
  @router.get("/admin/users")
  def admin_get_users(
      current_user: User = Depends(get_current_admin_user),
      db: Session = Depends(get_db)
  ):
      # admin만 접근 가능!
      return db.query(User).all()
  ```
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

## Day 14: 로깅, 미들웨어, 비동기, 테스팅

### 1교시: Day 13 복습 + 로깅 기초 시작

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

### 3교시: 로깅 실전 ⭐⭐⭐

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

### 4교시: 커스텀 미들웨어 ⭐⭐

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

### 6교시: 백그라운드 태스크 + Health Check ⭐⭐

- **백그라운드 태스크 (30min)**:
  - **개념 (10min)**:
    - BackgroundTasks
    - 비동기 작업 처리
    - 사용 사례
  - **Basic (15min)**:
    - BackgroundTasks 사용
    - 이메일 전송 예시
    - 로그 기록
  - **Practice (5min)**:
    - 백그라운드 작업 구현

- **Health Check 엔드포인트 (10min)**:
  - **개념 (3min)**:
    - 왜 필요한가? (모니터링, 로드밸런서)
    - 서비스 상태 확인
  - **Basic (5min)**:
    ```python
    @app.get("/health")
    def health_check():
        return {
            "status": "healthy",
            "timestamp": datetime.now().isoformat()
        }
    
    # DB 연결 체크 포함
    @app.get("/health/detailed")
    def detailed_health_check(db: Session = Depends(get_db)):
        try:
            # DB 연결 테스트 (SQLAlchemy)
            db.execute("SELECT 1")
            db_status = "healthy"
        except Exception:
            db_status = "unhealthy"
        
        return {
            "status": "healthy" if db_status == "healthy" else "degraded",
            "database": db_status,
            "timestamp": datetime.now().isoformat()
        }
    ```
  - **Practice (2min)**:
    - Health Check 엔드포인트 추가

- **Exercise (10min)**:
  - 백그라운드 이미지 처리

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

### 8교시: 테스팅 실전 + 파일 처리 ⭐⭐⭐

- **테스팅 실전 (30min)**:
  - 개념 (5min):
    - fixture
    - 테스트 DB 분리
    - 인증 테스트
  - Basic (15min):
    ```python
    import pytest
    from fastapi.testclient import TestClient
    from sqlalchemy import create_engine
    from sqlalchemy.orm import sessionmaker
    from app.database import Base, get_db
    from app.main import app
    
    # 테스트용 DB 설정
    SQLALCHEMY_DATABASE_URL = "sqlite:///./test.db"
    engine = create_engine(SQLALCHEMY_DATABASE_URL)
    TestingSessionLocal = sessionmaker(autocommit=False, autoflush=False, bind=engine)
    
    @pytest.fixture
    def client():
        # 테스트 DB 생성
        Base.metadata.create_all(bind=engine)
        
        # DB 의존성 오버라이드
        def override_get_db():
            try:
                db = TestingSessionLocal()
                yield db
            finally:
                db.close()
        
        app.dependency_overrides[get_db] = override_get_db
        
        yield TestClient(app)
        
        # 테스트 DB 삭제
        Base.metadata.drop_all(bind=engine)
    
    def test_create_user(client):
        response = client.post(
            "/users",
            json={"email": "test@example.com", "password": "test123"}
        )
        assert response.status_code == 201
    
    def test_with_auth(client):
        # 1. 회원가입
        client.post("/users", json={"email": "admin@test.com", "password": "admin"})
        
        # 2. 로그인
        login_response = client.post(
            "/auth/login",
            data={"username": "admin@test.com", "password": "admin"}
        )
        token = login_response.json()["access_token"]
        
        # 3. 인증된 요청
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

---

## Day 15: 심화 완성 + 최종 프로젝트

### 1교시: Day 14 복습 + 심화 마무리

- **복습 퀴즈 (10min)**: 로깅, 미들웨어, 테스팅
- **핵심 복습 (15min)**:
  - 로깅 전략 복습
  - pytest 복습
  - 간단한 Q&A
- **심화 과정 마무리 (25min)**:
  - 지금까지 배운 내용 정리
  - 프로덕션 레벨 체크리스트
  - 실무 적용 방법

### 2교시: 심화 주제 1 - 캐싱 기초 ⭐⭐

- **개념 (10min)**:
  - 캐싱이란? 성능 최적화
  - 언제 필요한가?
  - TTL (Time To Live)
  - Redis 맛보기
- **Basic (25min)**:
  - 간단한 메모리 캐싱
  - functools.lru_cache
  - FastAPI에서 캐싱 패턴
  - 실전 예제:
    ```python
    from functools import lru_cache
    
    @lru_cache(maxsize=128)
    def get_expensive_data(query: str):
        # 비용이 큰 연산
        return result
    ```
- **Practice (10min)**:
  - API 응답 캐싱
  - 계산 결과 캐싱
- **Exercise (5min)**:
  - 캐싱 전략 설계

### 3교시: 심화 주제 2 - 배포 개념 ⭐⭐

- **개념 (15min)**:
  - 로컬 vs 프로덕션
  - 배포란?
  - 클라우드 서비스 (AWS, GCP, Azure)
  - 도메인과 HTTPS
- **Basic (20min)**:
  - uvicorn 프로덕션 설정
  - 환경 변수 관리 (실전)
  - 로그 설정
  - gunicorn (간단히)
- **Practice (10min)**:
  - 프로덕션 설정 파일 작성
  - 배포 체크리스트
- **Exercise (5min)**:
  - 배포 전 준비사항 정리

### 4교시: 심화 주제 3 - Docker 맛보기 ⭐⭐

- **개념 (10min)**:
  - Docker란?
  - 컨테이너화의 장점
  - 이미지와 컨테이너
  - 왜 필요한가?
- **Basic (25min)**:
  - Dockerfile 기본:
    ```dockerfile
    FROM python:3.11-slim
    
    WORKDIR /app
    
    COPY requirements.txt .
    RUN pip install --no-cache-dir -r requirements.txt
    
    COPY . .
    
    CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
    ```
  - 이미지 빌드 개념
  - 컨테이너 실행 개념
- **Practice (10min)**:
  - Dockerfile 작성
  - requirements.txt 정리
- **Exercise (5min)**:
  - Docker 명령어 학습

### 5교시: 프로젝트 기획 및 설계 ⭐⭐⭐

- **요구사항 분석 (20min)**:
  - 기능 목록 작성
  - 우선순위 결정 (MVP)
  - 로깅 전략
  - 테스트 범위
  - **필수**: SQLAlchemy 모델, 로깅, 기본 테스트 포함

- **API 설계 (20min)**:
  - 엔드포인트 설계
  - Request/Response 모델 (Pydantic)
  - 인증/권한 설계

- **DB 스키마 설계 (10min)**:
  - SQLAlchemy 모델 구조
  - 관계 설정 (relationship)

### 6교시: 프로젝트 구현 (1) - 기본 구조 ⭐⭐⭐

- **프로젝트 초기화 (15min)**:
  - 디렉터리 구조 (3계층)
  - 가상환경
  - 설정 파일 (.env)
  - 로거 설정

- **SQLAlchemy 모델 작성 (20min)**:
  - Base 설정
  - 모델 정의 (relationship 포함)
  - 테이블 생성

- **기본 CRUD (15min)**:
  - 핵심 엔드포인트 구현

### 7교시: 프로젝트 구현 (2) - 인증 및 핵심 기능 ⭐⭐⭐

- **사용자 모델 (10min)**:
  - User 모델 (SQLAlchemy)
  - 패스워드 해싱

- **인증 구현 (20min)**:
  - 회원가입
  - 로그인
  - JWT

- **핵심 기능 시작 (20min)**:
  - 주요 비즈니스 로직
  - Service 계층 활용
  - SQLAlchemy relationship 활용

### 8교시: 프로젝트 구현 (3) - 완성 및 코드 리뷰 ⭐⭐⭐

- **기능 완성 (30min)**:
  - 핵심 기능 완성
  - 검증 강화
  - 로깅 추가
  - 에러 처리

- **테스트 작성 (10min)**:
  - 주요 엔드포인트 테스트
  - pytest 실행

- **코드 리뷰 + 회고 (10min)**:
  - 코드 정리
  - 개인별 피드백
  - 배운 점 공유
  - 향후 학습 방향

---

## 📌 핵심 학습 목표

### 최우선 항목 ⭐⭐⭐

1. **프로젝트 구조**: 계층 분리 (Web-Service-Data)
2. **SQLAlchemy**: 모델, Session, CRUD, relationship
3. **의존성 주입**: FastAPI Depends, get_db() 패턴
4. **JWT 인증**: 회원가입, 로그인, 토큰 검증
5. **OAuth2 패턴**: 표준 인증 구현
6. **권한 관리**: 역할 기반 접근 제어
7. **환경 변수**: 설정 관리, 보안
8. **로깅**: 기초 + 실전 (프로덕션 필수!)
9. **테스팅**: 기초 + 실전 (프로덕션 필수!)
10. **전역 에러 핸들러**: 일관된 에러 응답
11. **커스텀 미들웨어**: 요청/응답 처리
12. **Health Check**: 서비스 모니터링

### 중요 항목 ⭐⭐

1. 비동기 프로그래밍 (개념 이해)
2. CORS 설정
3. 파일 업로드/다운로드
4. 백그라운드 태스크
5. 캐싱 기초
6. 배포 개념
7. Docker 맛보기

### 기본 항목 ⭐

1. httpx 활용
2. 성능 최적화 개념

---

## 🎓 학습 후 다음 단계

### 권장 학습 주제

1. **SQLAlchemy 심화**:
   - 복잡한 쿼리 (join, group_by, having)
   - Alembic 마이그레이션
   - 성능 최적화 (lazy loading, eager loading)

2. **비동기 SQLAlchemy** (선택):
   - async/await with SQLAlchemy
   - AsyncSession
   - 성능 향상

3. **심화 테스팅**:
   - 테스트 커버리지
   - Mock/Stub
   - 통합 테스트

4. **배포 실전**:
   - Docker 실습
   - CI/CD
   - 클라우드 배포 (AWS, GCP)

5. **모니터링**:
   - 로그 분석
   - 성능 모니터링
   - 알림 시스템

6. **Redis 캐싱**:
   - Redis 설치 및 사용
   - 캐싱 전략
   - Session 관리

---
