# Python 기초 과정 커리큘럼 v4.0

## 📋 과정 개요

- **과정명**: Python 기초 과정
- **목표**: FastAPI 개발에 필요한 Python 핵심 문법 습득
- **기간**: 5일 (Day 1 ~ Day 5)
- **일일 시간**: 8교시 (명목상 50분 × 8 = 400분, 실제 약 7시간)
- **총 시간**: 약 35시간
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
- 개념: 5-10분
- Basic: 15-25분
- Practice: 10-20분
- Exercise: 5-10분

**8교시 종합 실습 (50분)**
- 복습 퀴즈: 10분
- 🟢 기초 Problem: 15분
- 🟡 응용 Problem: 15분
- 🔴 도전 Problem: 10분

**복습 교시 (Day 2부터 매일 1교시, 50분)**
- 퀴즈: 20분
- 실습 복습: 25분
- Q&A: 5분

---

## 📌 사전 과제 (Day 1 시작 전)

### 환경 구축 (예상 60분)

**필수 설치 항목**
1. **Python 3.11 이상**: https://www.python.org/downloads/
2. **VS Code**: https://code.visualstudio.com/
3. **Git Bash**: https://git-scm.com/downloads
4. **Jupyter Notebook**: `pip install jupyter`

**설치 확인**
```bash
# Python 버전 확인
python --version

# pip 확인
pip --version

# Jupyter 실행 테스트
jupyter notebook
```

**트러블슈팅 가이드 제공**
- Python PATH 설정 방법
- pip 설치 오류 해결
- VS Code Python 확장 설치
- Git Bash 기본 명령어

---

## Day 1: Python 시작과 기본 자료형

### 1교시: Python 첫걸음 ⭐⭐
- **개념 (10분)**: 오리엔테이션, Python 특징, 실행 방법, FastAPI 로드맵 소개
- **Basic (15분)**: print(), 주석(#, """), 간단한 계산
- **Practice (20분)**: 자기소개 출력, 계산 실습, 여러 줄 주석
- **Exercise (5분)**: 회사 정보 출력

### 2교시: 변수와 숫자형 + type() ⭐⭐
- **개념 (8분)**: 변수 개념, 메모리, int/float, type() 함수로 타입 확인
- **Basic (18분)**: 변수 선언, type() 확인, 사칙 연산, 복합 연산자 (+=, -=)
- **Practice (15분)**: 나이 계산, 온도 변환, type() 실습
- **Exercise (9분)**: 쇼핑몰 가격 계산

### 3교시: 문자열 기본 ⭐⭐
- **개념 (7분)**: 문자열 개념, 작은따옴표/큰따옴표, 인덱싱, 슬라이싱
- **Basic (20분)**: 
  - 문자열 생성 (' vs ")
  - 문자열 연산 (+, *)
  - 인덱싱 [0], [-1]
  - 슬라이싱 [start:end]
- **Practice (15분)**: 
  - 이메일 주소 분리 (@ 기준)
  - 파일명 확장자 추출
  - 문자열 역순 출력
- **Exercise (8분)**: 전화번호 포맷팅 (010-1234-5678)

### 4교시: 문자열 메서드 ⭐⭐
- **개념 (5분)**: 메서드 개념, 점(.) 표기법, 자주 쓰는 메서드
- **Basic (22분)**: 
  - upper(), lower(), capitalize()
  - strip(), lstrip(), rstrip()
  - split(), join()
  - replace()
  - find(), count()
- **Practice (15분)**: 
  - 데이터 정제 (공백 제거)
  - CSV 파싱 (split)
  - 문자열 변환 (replace)
- **Exercise (8min)**: 이메일 검증 (소문자 변환 + @ 확인)

### 5교시: f-string 기본 ⭐⭐⭐
- **개념 (5분)**: 문자열 포매팅 필요성, f-string 사용 이유
- **Basic (20분)**: 
  - f-string 기본 문법 f"{변수}"
  - 표현식 포함 f"{1 + 1}"
  - 변수와 텍스트 혼합
  - 간단한 포매팅 :.2f (소수점)
- **Practice (15min)**: 
  - 상품 정보 출력
  - 계산 결과 포매팅
  - 사용자 인사말
- **Exercise (10분)**: 성적표 출력 (평균 소수점 2자리)

> **참고**: 복잡한 포매팅 (정렬, 패딩 등)은 필요할 때 찾아보면 됨

### 6교시: Boolean + 비교 연산자 + Truthy/Falsy ⭐⭐⭐
- **개념 (8min)**: Boolean 타입, True/False, 조건 판단의 기초
- **Basic (20분)**: 
  - True, False 값
  - 비교 연산자 (==, !=, <, >, <=, >=)
  - 논리 연산자 (and, or, not)
  - **Truthy/Falsy 맛보기 (5분)**:
    ```python
    # False로 취급되는 값들
    if "":        # 빈 문자열
    if 0:         # 숫자 0
    if []:        # 빈 리스트
    if None:      # None
    
    # True로 취급되는 값들  
    if "hello":   # 문자열
    if 1:         # 0이 아닌 숫자
    if [1, 2]:    # 리스트
    ```
- **Practice (15분)**: 
  - 나이 비교
  - 로그인 검증 (and 사용)
  - 간단한 조건 체크
- **Exercise (7분)**: 
  - 비밀번호 강도 체크 (길이 >= 8 and 특수문자 포함)
  - 할인 대상 판단

> **주의**: Truthy/Falsy는 맛보기만! 실제 활용은 Day 3 if문에서 제대로 배움

### 7교시: 입출력 + 형변환 ⭐⭐
- **개념 (7분)**: input() 특징 (항상 문자열), 형변환 필요성
- **Basic (18분)**: 
  - input() 기본
  - int(), str(), float() 형변환
  - 안전한 변환 (try-except 간단히)
  - 형변환 주의점
- **Practice (15분)**: 
  - 나이 입력받아 계산
  - BMI 계산기
  - 두 숫자 덧셈
- **Exercise (10분)**: 
  - 거스름돈 계산기 (입력 + 연산 + 출력)
  - 온도 변환기

### 8교시: Day 1 종합 실습
- **복습 퀴즈 (10분)**: Day 1 핵심 내용 (변수, 문자열, f-string, Boolean)
- **🟢 기초 Problem (15분)**: 프로필 카드 생성기 
  - 입력: 이름, 나이, 이메일
  - 출력: f-string으로 카드 형식
- **🟡 응용 Problem (15분)**: 쇼핑몰 영수증
  - 상품명, 가격, 수량 입력
  - 총액, 할인 계산
  - 포매팅 출력
- **🔴 도전 Problem (10분)**: 스마트 계산기
  - 사칙연산 선택
  - 입력 검증 (숫자인지 확인)
  - 0으로 나누기 방지

---

## Day 2: 컬렉션 자료형

### 1교시: Day 1 복습
- **퀴즈 (20분)**: 변수, f-string, Boolean, 형변환, Truthy/Falsy
- **실습 복습 (25분)**: 어제 Exercise 재도전
- **Q&A (5분)**

### 2교시: 리스트 기본 ⭐⭐
- **개념 (7분)**: 리스트 개념, 여러 값 저장, FastAPI 배열 처리
- **Basic (18분)**: 생성, 인덱싱, 슬라이싱, 연산 (+, *)
- **Practice (15분)**: 학생 점수 관리, 슬라이싱 연습
- **Exercise (10분)**: 성적 처리 (평균, 최고점)

### 3교시: 리스트 수정 ⭐⭐
- **개념 (5분)**: 리스트 가변성, 복사 주의
- **Basic (17분)**: 요소 추가/수정/삭제, del, 얕은 복사
- **Practice (18분)**: TODO 리스트, 장바구니
- **Exercise (10분)**: 학생 명단 관리

### 4교시: 리스트 메서드 ⭐⭐
- **개념 (5분)**: 핵심 메서드 소개
- **Basic (20분)**: append/extend, remove/pop, sort, index
- **Practice (15분)**: 점수 추가/삭제, 정렬
- **Exercise (10분)**: 재고 관리

### 5교시: 튜플 + 집합 ⭐⭐
- **개념 (8분)**: 튜플 불변성, 집합 중복 제거와 빠른 검색
- **Basic - 튜플 (15분)**: 생성, 언패킹, 활용 사례
- **Basic - 집합 (12분)**: 
  - set() 생성
  - 중복 자동 제거 (핵심!)
  - in 연산자로 빠른 검색 (O(1))
  - add(), remove() 간단히
  - **집합 연산은 제외** (합집합, 교집합 등은 실무에서 거의 안 씀)
- **Practice (10분)**: 
  - 좌표 처리 (튜플)
  - 태그 중복 제거 (집합)
  - 허용 사용자 목록 (집합 + in)
- **Exercise (5분)**: 
  - 함수 리턴값 (튜플)
  - 유니크 데이터 추출 (집합)

### 6교시: 딕셔너리 개념 ⭐⭐⭐
- **개념 (10분)**: key-value, JSON 구조 미리보기, FastAPI 핵심
- **Basic (22분)**: 생성, 접근, 추가/수정/삭제, in 연산자
- **Practice (13분)**: 학생 정보, 상품 재고
- **Exercise (5분)**: 연락처 관리

### 7교시: 딕셔너리 메서드 ⭐⭐⭐
- **개념 (5분)**: get()의 중요성 (KeyError 방지)
- **Basic (22분)**: keys/values/items, get, pop/update
- **Practice (15분)**: 딕셔너리 순회, 안전한 접근
- **Exercise (8분)**: API 응답 처리 (딕셔너리 조합)

### 8교시: Day 2 종합 실습
- **복습 퀴즈 (10분)**: 리스트, 튜플, 집합, 딕셔너리
- **🟢 기초 Problem (15분)**: 학생 관리 (딕셔너리)
- **🟡 응용 Problem (20분)**: 상품 재고 관리 (딕셔너리 + 리스트)
- **🔴 도전 Problem (5분)**: 데이터 변환 및 통계

---

## Day 3: 딕셔너리 심화와 제어문

### 1교시: Day 2 복습
- **퀴즈 (20분)**: 컬렉션 전체
- **실습 복습 (25분)**: 딕셔너리 집중
- **Q&A (5분)**

### 2교시: 딕셔너리 심화 (1) - 중첩 ⭐⭐⭐
- **개념 (10분)**: 중첩 딕셔너리, JSON 구조
- **Basic (20분)**: 중첩 딕셔너리 생성/접근, JSON 예제
- **Practice (13분)**: 사용자 프로필, API 응답 파싱
- **Exercise (7분)**: 복잡한 데이터 구조 다루기

### 3교시: 딕셔너리 심화 (2) - 언패킹 ⭐⭐⭐
- **개념 (10분)**: 딕셔너리 언패킹, **kwargs 미리보기
- **Basic (22분)**: 언패킹 활용, 딕셔너리 병합
- **Practice (13분)**: 설정 데이터 병합
- **Exercise (5분)**: 여러 딕셔너리 합치기

### 4교시: 조건문 (if) + Truthy/Falsy 실전 ⭐⭐⭐
- **개념 (10분)**: 조건문 필요성, 논리 흐름
- **Basic (22분)**: 
  - if/elif/else 기본
  - 논리 연산자 (and, or, not)
  - **Truthy/Falsy 실전 활용**:
    ```python
    # Day 1 맛보기 복습 + 실전 활용
    if name:              # 빈 문자열 체크
    if items:             # 빈 리스트 체크
    if not data:          # 데이터 없음 체크
    if user and user.get("active"):  # 안전한 접근
    ```
  - in 연산자 활용
- **Practice (13분)**: 
  - 성적 등급
  - 로그인 검증
  - 안전한 데이터 접근
- **Exercise (5분)**: 할인율 계산, 접근 권한 체크

### 5교시: for문 ⭐⭐⭐
- **개념 (7분)**: 반복문, FastAPI 활용 (리스트 처리)
- **Basic (22분)**: for 기본, range(), enumerate(), items()
- **Practice (13분)**: 리스트 순회, 딕셔너리 출력
- **Exercise (8분)**: 합계, 필터링

### 6교시: while문 ⭐⭐
- **개념 (5분)**: while문, for vs while
- **Basic (18분)**: while 기본, break/continue, 재시도 로직
- **Practice (17분)**: 숫자 맞추기, 메뉴 시스템
- **Exercise (10분)**: 비밀번호 재입력

### 7교시: 리스트 컴프리헨션 ⭐⭐
- **개념 (7분)**: 컴프리헨션, 간결한 코드
- **Basic (20분)**: 기본 문법, 조건문 포함
- **Practice (15분)**: 데이터 변환, 필터링
- **Exercise (8분)**: 짝수 추출, 대문자 변환

### 8교시: Day 3 종합 실습
- **복습 퀴즈 (10분)**: 딕셔너리, 제어문, Truthy/Falsy
- **🟢 기초 Problem (15분)**: 메뉴 선택 (while + 딕셔너리)
- **🟡 응용 Problem (20분)**: 성적 처리 (for + 딕셔너리 + 컴프리헨션)
- **🔴 도전 Problem (5분)**: 간단한 게임

---

## Day 4: 함수 완전 정복 ⭐⭐⭐

### 1교시: Day 3 복습
- **퀴즈 (20분)**: 딕셔너리 심화, 제어문
- **실습 복습 (25분)**: 반복문 집중
- **Q&A (5분)**

### 2교시: 함수 기본 ⭐⭐
- **개념 (8분)**: 함수 필요성, FastAPI 엔드포인트와의 관계
- **Basic (18분)**: def, 호출, return, 여러 개 반환 (튜플)
- **Practice (15분)**: 계산 함수, 문자열 처리
- **Exercise (9분)**: 온도 변환 함수

### 3교시: 매개변수 (1) - 위치와 기본값 + None ⭐⭐⭐
- **개념 (10분)**: 매개변수 vs 인수, 기본값, None의 활용
- **Basic (22분)**: 
  - 위치 인수
  - 기본값 (숫자, 문자열)
  - **None 기본값 패턴** (중요!):
    ```python
    def get_user(user_id: int, default=None):
        # None으로 "값 없음"을 표현
        if user not found:
            return default
    
    def create_profile(name: str, bio: str = None):
        # 선택적 매개변수
        if bio is None:
            bio = "소개가 없습니다"
    ```
  - 조합
- **Practice (13분)**: 
  - 인사 함수
  - 프로필 출력
  - None 처리 연습
- **Exercise (5분)**: 등급 계산 (기본값 활용)

### 4교시: 매개변수 (2) - 키워드 인수 ⭐⭐⭐
- **개념 (8분)**: 키워드 인수, FastAPI 쿼리 파라미터와의 관계
- **Basic (20분)**: 키워드 인수, 혼합, 실전 예제
- **Practice (14분)**: API 스타일 함수
- **Exercise (8분)**: 사용자 생성 함수

### 5교시: 가변 인수 ⭐⭐⭐
- **개념 (10분)**: *args, **kwargs, FastAPI 핵심
- **Basic (22분)**: *args, **kwargs, 조합, 언패킹
- **Practice (10분)**: 합계 함수, 로그 함수
- **Exercise (8분)**: 유연한 계산기

### 6교시: 람다와 스코프 ⭐⭐
- **개념 (5분)**: 스코프, 람다
- **Basic (20분)**: 지역/전역 변수, lambda, map/filter
- **Practice (15분)**: 변수 스코프, 람다 활용
- **Exercise (10분)**: 정렬 키

### 7교시: 예외 처리 + isinstance() ⭐⭐
- **개념 (8분)**: 예외 처리, FastAPI HTTPException 미리보기
- **Basic (20분)**: 
  - try-except 기본
  - Exception as e
  - finally
  - raise
  - **isinstance() 간단히 (5분)**:
    ```python
    # 타입 체크 방법도 있다 정도만
    try:
        result = int(value)
    except ValueError:
        if isinstance(value, str):
            print("문자열입니다")
    ```
- **Practice (15분)**: 안전한 입력, 검증
- **Exercise (7분)**: 나누기 함수 (0 체크)

> **참고**: isinstance()는 깊게 안 다룸. Pydantic이 타입 검증 자동으로 해줌!

### 8교시: Day 4 종합 실습
- **복습 퀴즈 (10분)**: 함수 전체
- **🟢 기초 Problem (15분)**: 계산기 함수 모음 (*args 활용)
- **🟡 응용 Problem (20분)**: 데이터 검증 시스템 (**kwargs 활용)
- **🔴 도전 Problem (5분)**: 유연한 API 함수 (None 처리 포함)

---

## Day 5: 클래스와 타입 힌트 ⭐⭐⭐

### 1교시: Day 4 복습
- **퀴즈 (20분)**: 함수, 가변 인수, None 처리
- **실습 복습 (25분)**: *args, **kwargs 집중
- **Q&A (5분)**

### 2교시: 클래스 기본 ⭐⭐
- **개념 (10분)**: OOP 개념, 클래스 vs 객체, Pydantic BaseModel 미리보기
- **Basic (20분)**: class 정의, __init__, self, 인스턴스
- **Practice (13분)**: 학생 클래스, 계좌 클래스
- **Exercise (7분)**: 상품 클래스

### 3교시: 클래스 활용 ⭐⭐
- **개념 (7분)**: 인스턴스 메서드, 클래스 활용
- **Basic (20분)**: 메서드 작성, 상태 변경, 데이터 캡슐화
- **Practice (15분)**: TODO 클래스, 메서드 활용
- **Exercise (8분)**: 유저 클래스

### 4교시: 타입 힌트 (1) - 기본 ⭐⭐⭐
- **개념 (10분)**: 타입 힌트 필요성, FastAPI/Pydantic 핵심!
- **Basic (22분)**: 
  - int, str, float, bool
  - 함수 타입 힌트 (매개변수, 반환값)
  - 타입 힌트는 "힌트"일 뿐 (강제 X)
- **Practice (13분)**: 타입 힌트 추가 연습
- **Exercise (5분)**: 기존 코드에 타입 추가

### 5교시: 타입 힌트 (2) - 고급 ⭐⭐⭐
- **개념 (10분)**: 복잡한 타입, Optional 중요성
- **Basic (20분)**: 
  - List[int], Dict[str, int]
  - **Optional[str]** (핵심!)
  - Union[int, str]
  - 타입 힌트 조합
- **Practice (13분)**: 복잡한 타입 작성
- **Exercise (7분)**: API 응답 타입 (간단히)

### 6교시: 데코레이터 ⭐⭐
- **개념 (10분)**: 데코레이터 개념, @app.get 미리보기
- **Basic (20분)**: 데코레이터 기본, 간단한 예제
- **Practice (15분)**: 로깅 데코레이터
- **Exercise (5분)**: 타이머 데코레이터

### 7교시: import 완전 정복 ⭐⭐⭐
- **개념 (10분)**: 
  - 모듈이란? 재사용 가능한 코드
  - 왜 필요? (Django/FastAPI 프로젝트 구조)
  - 남의 코드 vs 내 코드
- **Basic (22분)**: 
  - import 기본: `import json`
  - from import: `from json import dumps, loads`
  - 별칭: `import math as m`
  - 표준 라이브러리 활용 (datetime, random 등)
  - **내 파일 import** (같은 디렉토리):
    ```python
    # calculator.py
    def add(a, b):
        return a + b
    
    # main.py
    import calculator
    print(calculator.add(1, 2))
    ```
- **Practice (13min)**: 
  - 계산기 모듈 만들기 (calculator.py)
  - 유틸리티 모듈 만들기 (utils.py)
  - 다른 파일에서 import해서 사용
- **Exercise (5분)**: 
  - 검증 함수 모듈 작성 (validators.py)
  - 메인 파일에서 import하여 활용

> **중요**: JSON은 Day 6 웹 과정에서 배움! (웹 맥락과 함께)

### 8교시: 기초 과정 종합 실습 ⭐⭐⭐
- **복습 퀴즈 (10분)**: Day 1-5 핵심 개념
- **🟢 기초 Problem (15분)**: 클래스 + 타입 힌트 시스템
  - 학생 클래스에 타입 힌트 추가
  - 메서드 구현
- **🟡 응용 Problem (20분)**: 모듈화 프로젝트
  - 여러 모듈로 분리 (models.py, utils.py, main.py)
  - 타입 힌트 적용
  - import로 연결
- **🔴 도전 Problem (5분)**: 창의적 확장
  - 데코레이터 + 클래스 조합
  - 복잡한 타입 힌트

---

## 📌 핵심 학습 목표 (FastAPI 중심)

### 최우선 항목 ⭐⭐⭐
1. **딕셔너리**: JSON의 기초, API 데이터 구조
2. **타입 힌트**: Pydantic 모델의 핵심
3. **함수 (매개변수, *args, **kwargs)**: 엔드포인트 작성
4. **클래스 (기초)**: Pydantic BaseModel 이해
5. **None과 Optional**: 선택적 필드 처리
6. **데코레이터 개념**: @app.get, @app.post 이해
7. **import**: 모듈화, FastAPI 프로젝트 구조

### 중요 항목 ⭐⭐
1. 리스트
2. 조건문, 반복문
3. 예외 처리
4. 문자열 (f-string)
5. Boolean, Truthy/Falsy

### 기본 항목 ⭐
1. 튜플
2. 집합 (중복 제거, 빠른 검색)
3. while문
4. 람다 함수
5. isinstance() (간단히만)

---

## 💡 교육 운영 팁

### 준비 사항
- [ ] 사전 과제 설치 가이드 (동영상 or PDF)
- [ ] 각 일차별 PPT 슬라이드
- [ ] 각 일차별 Jupyter Notebook 파일
- [ ] 전체 정답 코드
- [ ] 트러블슈팅 FAQ

### 파일 구조
```
Day1_Python기초/
├── slides/
│   └── Day1_전체.pptx
├── notebooks/
│   ├── 01_개념_첫걸음.ipynb
│   ├── 02_Basic_변수.ipynb
│   ├── 03_Practice_변수.ipynb
│   ├── 04_Exercise_변수.ipynb
│   └── ...
├── solutions/
│   ├── Practice_정답.ipynb
│   ├── Exercise_정답.ipynb
│   └── Problem_정답.ipynb
└── README.md

Day5_클래스와타입/
├── modules_example/
│   ├── calculator.py
│   ├── validators.py
│   └── main.py
└── ...
```

### Jupyter vs .py 파일 사용 가이드
- **Day 1-2**: Jupyter 노트북 위주 (즉각적 피드백)
- **Day 3**: 혼용 (딕셔너리는 Jupyter, 제어문은 .py)
- **Day 4-5**: .py 파일 중심 (실무 환경 적응, 모듈 만들기)

### 난이도 표시
- 🟢 기초: 오늘 배운 내용만
- 🟡 응용: 이전 내용 + 오늘 내용
- 🔴 도전: 창의적 사고 필요

---

## 🔧 트러블슈팅 가이드

### 자주 발생하는 문제

**1. Python PATH 설정 안 됨**
```bash
# Windows
시스템 환경 변수 편집 → Path 추가

# 확인
python --version
```

**2. pip 설치 오류**
```bash
# pip 업그레이드
python -m pip install --upgrade pip

# Jupyter 설치
pip install jupyter
```

**3. Jupyter 실행 안 됨**
```bash
# Jupyter 재설치
pip uninstall jupyter
pip install jupyter

# 실행
jupyter notebook
```

**4. VS Code Python 인식 안 함**
- Python 확장 설치: ms-python.python
- 인터프리터 선택: Ctrl+Shift+P → "Python: Select Interpreter"

**5. 인코딩 오류 (Windows)**
```python
# 파일 열 때 encoding 지정
with open('file.txt', 'r', encoding='utf-8') as f:
    data = f.read()
```

**6. import 오류**
```python
# ModuleNotFoundError
# → 같은 디렉토리에 파일이 있는지 확인
# → 파일명과 import명이 일치하는지 확인
```

---

## 📚 참고 자료

### 교재
- 점프 투 파이썬 (박응용)
- 처음 시작하는 파이썬
- 처음 시작하는 FastAPI (빌 루바노빅)

### 온라인 리소스
- Python 공식 문서: https://docs.python.org/3/
- FastAPI 공식 문서: https://fastapi.tiangolo.com/
- Pydantic 공식 문서: https://docs.pydantic.dev/

### 추천 도구
- Jupyter Notebook
- VS Code
- Git Bash

---

## 🎓 평가 기준

### 출석 및 참여 (30%)
- 매일 출석
- 실습 참여도
- 사전 과제 완료

### 실습 과제 (40%)
- Exercise 완성도
- 종합 Problem 해결

### 응용 과정 준비도 (30%)
- 딕셔너리 이해도
- 타입 힌트 활용
- 함수 작성 능력
- import 이해

---

## 🎯 기초 과정 완료 후 체크리스트

### 학생이 할 수 있어야 하는 것:
- [ ] 변수, 자료형 자유롭게 사용
- [ ] f-string으로 포매팅
- [ ] 딕셔너리 생성, 접근, 수정
- [ ] 중첩 딕셔너리 다루기
- [ ] for/while 반복문 작성
- [ ] 함수 정의, 매개변수 활용
- [ ] *args, **kwargs 이해
- [ ] None 처리
- [ ] 간단한 클래스 작성
- [ ] 타입 힌트 추가 (기본 + Optional)
- [ ] import로 모듈 사용
- [ ] 내 모듈 만들고 import하기
- [ ] 예외 처리 (try-except)
- [ ] Truthy/Falsy 활용

### 응용 과정 준비 상태:
- [ ] FastAPI 설치 준비 완료
- [ ] 타입 힌트 익숙함
- [ ] 딕셔너리 자유자재
- [ ] 함수 패턴 이해
- [ ] 모듈 구조 이해
- [ ] JSON 배울 준비 완료 (Day 6에서)

---

## 📝 v3에서 v4 주요 변경사항

### 구조 변경
1. **Day 1-7교시**: 복습 제거 → 입출력 + 형변환
2. **Day 1 재구성**: 
   - 문자열 3-4교시로 분리
   - f-string 난이도 하향 (기본)
   - Boolean 독립 교시 (Truthy/Falsy 맛보기 포함)
3. **Day 5-7교시**: JSON 제거, import 완전 정복
4. **Day 2-5교시**: 집합 시간 확대 (7분 → 12분), 연산 제외
5. **Day 4-7교시**: isinstance() 5분만 (예외 처리에서)

### 내용 개선
- Truthy/Falsy: Day 1 맛보기 + Day 3 실전
- None 기본값: Day 4-3교시에서 명확히
- import: 실무 중심 (모듈 만들기)
- 집합: 중복 제거 + 빠른 검색만 (연산 제외)
- isinstance(): 최소화 (Pydantic이 대체)

### 시간 최적화
- Day 1: 복습 제거로 여유 확보
- 각 교시: 압축 해소, 자연스러운 흐름

---

**최종 수정일**: 2026-01-29
**버전**: 4.0
**작성자**: FastAPI 교육 커리큘럼 팀
**다음 과정**: Python 응용 과정 v4.0 (Day 6-10)
