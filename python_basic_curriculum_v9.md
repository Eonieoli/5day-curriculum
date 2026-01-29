# Python 기초 과정 커리큘럼 v9.0

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
- Exercise: 10-15분

**8교시 종합 실습 (50분)**

- 복습 퀴즈: 10분
- 🟢 기초 Problem: 15분
- 🟡 응용 Problem: 15분
- 🔴 도전 Problem: 10분

**복습 교시 (Day 2부터 매일 1교시, 50분)**

- 복습 퀴즈: 10분 (간소화!)
- 핵심 복습: 15분 (전날 가장 중요한 것만!)
- 새 내용: 25분 (바로 진도!)

---

## Day 1: Python 시작과 기본 자료형

### 1교시: 환경 구축 (50분 전체) ⭐⭐⭐

- **Python 설치 확인 (10분)**:
  - Python 버전 확인 (`python --version`)
  - 설치 안 된 학생 개별 지도
  - 환경 변수 설정 확인
- **VS Code 설치 및 설정 (10분)**:
  - VS Code 설치 확인
  - Python 확장 설치
  - 기본 설정
- **Jupyter Notebook 설치 (10분)**:
  - `pip install jupyter`
  - 설치 확인
  - Jupyter 실행 테스트
- **Hello World + 주석 (10분)**:
  - `print("Hello, World!")`
  - 주석 (#, """)
  - 간단한 계산 테스트
- **트러블슈팅 (10분)**:
  - 개별 문제 해결
  - 모든 학생 동일한 환경 확인

> **중요**: 모든 학생이 동일한 환경에서 시작! 문제 있으면 즉시 해결!

### 2교시: 변수와 숫자형 ⭐⭐

- **개념 (8분)**: 
  - 변수 개념
  - 메모리 저장
  - int/float 타입
  - type() 함수
- **Basic (18분)**:
  - 변수 선언과 할당
  - type() 함수로 타입 확인
  - 사칙 연산 (+, -, \*, /, //, %, \*\*)
  - 복합 연산자 (+=, -=, \*=, /=)
- **Practice (12분)**:
  - 나이 계산
  - 온도 변환 (섭씨 → 화씨)
  - type() 확인 실습
- **Exercise (12분)**:
  - 쇼핑몰 가격 계산
  - BMI 계산기 (기본)

### 3교시: 문자열 기본 ⭐⭐

- **개념 (5분)**: 
  - 문자열 개념
  - 불변성
  - 작은따옴표/큰따옴표
- **Basic (20분)**:
  - 문자열 생성 (' vs ")
  - 문자열 연산 (+, \*)
  - len() 함수
  - 간단한 예제
- **Practice (15분)**:
  - 이름 합치기
  - 인사말 만들기
  - 문자열 반복으로 패턴 만들기
- **Exercise (10분)**:
  - 문자열 연산 활용
  - 길이 계산

### 4교시: 문자열 인덱싱/슬라이싱 ⭐⭐⭐

- **개념 (7분)**: 
  - 인덱스 개념
  - 음수 인덱스
  - 슬라이싱
- **Basic (23분)**:
  - 인덱싱 [0], [-1]
  - 슬라이싱 [start:end]
  - [start:], [:end], [::step]
  - [::-1] (역순)
- **Practice (12분)**:
  - 첫 글자/마지막 글자 추출
  - 전화번호 포맷팅 (010-1234-5678)
  - 파일명에서 확장자 추출
- **Exercise (8분)**:
  - 이메일에서 @ 앞부분 추출
  - 문자열 역순 출력

### 5교시: 문자열 메서드 ⭐⭐

- **개념 (5분)**: 
  - 메서드란?
  - 불변성 복습
- **Basic (20분)**:
  - `upper()`, `lower()`: 대소문자 변환
  - `strip()`: 공백 제거
  - `split()`: 문자열 분리
  - `replace()`: 문자열 교체
  - 실전 예제
- **Practice (15분)**:
  - CSV 데이터 파싱 (split)
  - 데이터 정제 (strip + lower)
  - 텍스트 치환 (replace)
- **Exercise (10분)**:
  - 복합 메서드 활용
  - 실전 데이터 처리

> **제거된 메서드**: capitalize, lstrip, rstrip, join, find, count
> → 필요할 때 공식 문서 보면 됨!

### 6교시: f-string ⭐⭐⭐

- **개념 (5분)**: 
  - 문자열 포매팅 필요성
  - f-string 장점
- **Basic (18분)**:
  - f-string 기본 문법: `f"{변수}"`
  - 표현식 포함: `f"{1 + 1}"`
  - 변수와 텍스트 혼합
  - 소수점 포매팅: `f"{pi:.2f}"`
- **Practice (15분)**:
  - 상품 정보 출력
  - 계산 결과 포매팅
  - 사용자 인사말 (이름 + 나이)
- **Exercise (12분)**:
  - 성적표 출력 (평균 소수점 2자리)
  - 영수증 출력 (상품명, 가격, 총액)

> **참고**: 복잡한 포매팅 (정렬, 패딩)은 필요할 때 찾아보면 됨

### 7교시: 입출력 + 형변환 ⭐⭐

- **개념 (7분)**: 
  - input() 특징 (항상 문자열)
  - 형변환 필요성
- **Basic (18분)**:
  - input() 기본
  - int(), str(), float() 형변환
  - 형변환 주의점
  - 간단한 에러 예시
- **Practice (13분)**:
  - 나이 입력받아 계산
  - BMI 계산기
  - 두 숫자 덧셈
- **Exercise (12분)**:
  - 거스름돈 계산기
  - 온도 변환기 (입력 포함)

### 8교시: Day 1 종합 실습

- **복습 퀴즈 (10분)**: 변수, 숫자형, 문자열, f-string, 형변환
- **🟢 기초 Problem (15분)**: 프로필 카드 생성기
  - 입력: 이름, 나이, 이메일
  - 출력: f-string으로 카드 형식
- **🟡 응용 Problem (15분)**: 쇼핑몰 영수증
  - 상품명, 가격, 수량 입력
  - 총액, 할인 계산
  - 포매팅 출력
- **🔴 도전 Problem (10분)**: 데이터 처리 프로그램
  - 문자열 메서드 + 형변환 + f-string 종합

---

## Day 2: 컬렉션 자료형

### 1교시: Day 1 복습 + 리스트 시작

- **복습 퀴즈 (10분)**: 변수, f-string, 문자열, 형변환
- **핵심 복습 (15분)**: 
  - f-string 실습 (가장 중요!)
  - 문자열 메서드 복습
  - 간단한 Q&A
- **리스트 기본 시작 (25분)**:
  - 개념 (7분): 리스트란? 여러 값 저장, FastAPI 배열 처리
  - Basic (18분):
    - 리스트 생성 `[]`
    - 인덱싱 `[0]`, `[-1]`
    - 슬라이싱 `[start:end]`
    - 연산 (+, \*)
    - **len() 함수** (리스트 길이)

### 2교시: 리스트 기본 + len() ⭐⭐

- **Basic 완성 (25분)**:
  - len() 활용 예제
  - 리스트 순회 미리보기
  - 실전 예제
- **Practice (15분)**:
  - 학생 점수 관리
  - 슬라이싱으로 일부 추출
  - len()으로 개수 확인
- **Exercise (10분)**:
  - 성적 처리 (평균 = sum/len)
  - 리스트 연산 활용

### 3교시: 리스트 수정 (메서드) ⭐⭐

- **개념 (5분)**: 리스트 가변성, 메서드란?
- **Basic (20분)**:
  - 요소 추가:
    - `list.append(value)`: 끝에 추가
    - `list.insert(index, value)`: 특정 위치 추가
  - 요소 수정: `list[0] = new_value`
  - 요소 삭제:
    - `del list[index]`: 인덱스로 삭제
    - `list.remove(value)`: 값으로 삭제
    - `list.pop()`: 마지막 제거 및 반환
    - `list.pop(index)`: 특정 위치 제거 및 반환
- **Practice (15분)**:
  - TODO 리스트 관리
  - 장바구니 추가/삭제
  - pop() 활용
- **Exercise (10분)**:
  - 학생 명단 관리
  - 재고 목록 수정

### 4교시: 내장 함수 + 리스트 순수 함수 ⭐⭐

- **개념 (7분)**: 내장 함수란? 순수 함수 vs 메서드 차이
- **Basic (23분)**:
  - **핵심 내장 함수** (15분):
    - `len()`: 길이 (복습)
    - `max()`, `min()`: 최댓값, 최솟값
    - `sum()`: 합계
    - `sorted()`: 정렬된 새 리스트 반환
  - **리스트 메서드 vs 순수 함수** (8분):
    - `sort()`: 제자리 정렬 (원본 변경)
    - `sorted()`: 새 리스트 반환 (원본 유지)
    - 차이점 이해하기
    - 얕은 복사 개념
- **Practice (12분)**:
  - 점수 통계 (max, min, sum 활용)
  - 정렬 비교 (sort vs sorted)
  - 리스트 복사 실험
- **Exercise (8분)**:
  - 성적 분석 (평균, 최고, 최저)
  - 순위 정렬

### 5교시: 튜플 + 집합 ⭐⭐

- **튜플 (30분)**:
  - **개념 (7분)**: 튜플 불변성, 언패킹, 활용 사례
  - **Basic (15분)**:
    - 튜플 생성 `()`, `tuple()`
    - 인덱싱 (리스트와 동일)
    - **언패킹 강화** `x, y = (1, 2)`
    - **함수에서 여러 값 리턴** (중요!)
    - 수정 불가 특징
  - **Practice (8분)**:
    - 좌표 처리 (x, y)
    - **함수 다중 리턴값** (강화!)
    - RGB 색상값
    - 여러 변수 동시 할당
- **집합 (20분)**:
  - **개념 (5분)**: 중복 제거, 빠른 검색 (O(1))
  - **Basic (10분)**:
    - `set()` 생성
    - 중복 자동 제거
    - `in` 연산자로 검색
    - `add()`, `remove()` 간단히
  - **Practice (3분)**:
    - 태그 중복 제거
    - 허용 사용자 목록 (set + in)
  - **Exercise (2min)**:
    - 중복 제거 실습

> **중요 변경**: 튜플 확대(언패킹, 다중 리턴), 집합 축소!
> **제거**: 집합 연산 (합집합, 교집합 등) → 실무에서 거의 안 씀!

### 6교시: 딕셔너리 기초 ⭐⭐⭐

- **개념 (10분)**: 
  - key-value 
  - JSON 구조 미리보기
  - FastAPI 핵심
- **Basic (20분)**:
  - 생성 `{}`
  - 접근 `dict["key"]`
  - 추가/수정
  - 삭제 `del`
  - `in` 연산자
- **Practice (12분)**:
  - 학생 정보 딕셔너리
  - 상품 데이터
- **Exercise (8분)**:
  - 사용자 프로필 만들기

### 7교시: 딕셔너리 메서드 ⭐⭐⭐

- **개념 (5분)**: get()의 중요성 (KeyError 방지)
- **Basic (22분)**:
  - `keys()`, `values()`, `items()`
  - `get(key, default)` (핵심!)
  - `pop(key)`
  - `update()`
  - in 연산자
- **Practice (13분)**:
  - 딕셔너리 순회 (items())
  - 안전한 접근 (get())
  - 여러 딕셔너리 병합
- **Exercise (10분)**:
  - 상품 재고 관리
  - API 응답 처리 (딕셔너리 조합)

### 8교시: Day 2 종합 실습

- **복습 퀴즈 (10분)**: 리스트, 튜플, 집합, 딕셔너리
- **🟢 기초 Problem (15분)**: 학생 관리 (딕셔너리)
- **🟡 응용 Problem (15분)**: 상품 재고 관리 (딕셔너리 + 리스트)
- **🔴 도전 Problem (10분)**: 데이터 변환 및 통계

---

## Day 3: 제어문 완전 정복

### 1교시: Day 2 복습 + Boolean 시작 ⭐⭐⭐

- **복습 퀴즈 (10분)**: 컬렉션 전체
- **핵심 복습 (15분)**: 
  - 딕셔너리 메서드 (items, get)
  - 리스트 vs 튜플 차이
  - 간단한 Q&A
- **Boolean + 비교 연산자 시작 (25분)**:
  - 개념 (10분): Boolean 타입, True/False, 조건 판단의 기초
  - Basic (15min):
    - True, False 값
    - 비교 연산자 (==, !=, <, >, <=, >=)
    - 간단한 조건 체크

### 2교시: Boolean + 비교 연산자 완성 ⭐⭐⭐

- **Basic 완성 (20min)**:
  - 논리 연산자 (and, or, not)
  - 조합 예제
  - 실전 패턴
- **Practice (20min)**:
  - 나이 비교 (성인인지 확인)
  - 로그인 검증 (아이디 and 비밀번호)
  - 범위 체크 (0 <= 점수 <= 100)
- **Exercise (10min)**:
  - 비밀번호 강도 체크 (길이 >= 8)
  - 할인 대상 판단 (나이 or 회원 여부)

### 3교시: 조건문 (if) + Truthy/Falsy ⭐⭐⭐

- **개념 (10min)**: 조건문 필요성, 논리 흐름
- **Basic (22min)**:
  - if/elif/else 기본
  - 논리 연산자 복습
  - **Truthy/Falsy** (여기서 처음!):

    ```python
    # False로 취급되는 값
    if "":        # 빈 문자열
    if 0:         # 숫자 0
    if []:        # 빈 리스트
    if {}:        # 빈 딕셔너리
    if None:      # None

    # True로 취급되는 값
    if "hello":   # 문자열
    if 1:         # 0이 아닌 숫자
    if [1, 2]:    # 리스트
    if {"a": 1}:  # 딕셔너리
    ```

  - in 연산자 활용

- **Practice (10min)**:
  - 성적 등급 (if/elif/else)
  - 로그인 검증
  - 빈 리스트 체크 (if items:)
- **Exercise (8min)**:
  - 할인율 계산
  - 안전한 데이터 접근 (if data:)

> **중요**: Truthy/Falsy를 if문과 함께 배우니 이해가 쉬움!

### 4교시: for문 기본 ⭐⭐⭐

- **개념 (7min)**: 반복문, FastAPI 활용 (리스트 처리)
- **Basic (23min)**:
  - for 기본 문법
  - range() (1개, 2개, 3개 인자)
  - 리스트 순회
  - 간단한 예제
- **Practice (12min)**:
  - 리스트 출력
  - range() 활용
  - 합계 계산
- **Exercise (8min)**:
  - 짝수만 출력
  - 구구단 (한 단)

### 5교시: for문 심화 ⭐⭐⭐

- **개념 (5min)**: enumerate, items, 중첩 for문
- **Basic (22min)**:
  - enumerate() (인덱스 + 값)
  - items() (딕셔너리)
  - break/continue
  - 중첩 for문 (간단히)
- **Practice (13min)**:
  - 딕셔너리 순회
  - enumerate 활용
  - 중첩 for문 (구구단)
- **Exercise (10min)**:
  - 조건부 순회
  - 2차원 데이터 처리

### 6교시: while문 ⭐⭐

- **개념 (5min)**: while문, for vs while
- **Basic (18min)**:
  - while 기본
  - break/continue
  - 재시도 로직
- **Practice (15min)**:
  - 숫자 맞추기 게임
  - 메뉴 시스템
- **Exercise (12min)**:
  - 비밀번호 재입력
  - 조건 만족까지 반복

### 7교시: 리스트 컴프리헨션 ⭐⭐

- **개념 (10min)**:
  - 왜 필요한가? 간결함, 성능
  - **FastAPI에서 자주 사용!**
  - for문 vs 컴프리헨션 비교
  - 기본 패턴 이해
- **Basic (20min)**:
  ```python
  # 기본 패턴
  numbers = [x for x in range(10)]
  
  # if 조건 포함
  evens = [x for x in range(10) if x % 2 == 0]
  
  # 변환
  squares = [x**2 for x in range(5)]
  
  # 문자열 리스트 변환
  names = ["alice", "bob", "charlie"]
  upper_names = [name.upper() for name in names]
  
  # 실전: API 응답 변환
  users = [{"name": "Alice", "age": 25}, {"name": "Bob", "age": 30}]
  names = [user["name"] for user in users]
  ages = [user["age"] for user in users if user["age"] >= 25]
  ```
- **Practice (12min)**:
  - 짝수 리스트
  - 제곱 리스트
  - 필터링 + 변환
- **Exercise (8min)**:
  - 복잡한 변환
  - 딕셔너리 리스트 처리

### 8교시: Day 3 종합 실습

- **복습 퀴즈 (10min)**: Boolean, if문, for문, while문, 컴프리헨션
- **🟢 기초 Problem (15min)**: 메뉴 선택 (while + if)
- **🟡 응용 Problem (15min)**: 성적 처리 (for + 딕셔너리 + 컴프리헨션)
- **🔴 도전 Problem (10min)**: 간단한 게임 (종합)

---

## Day 4: 함수 완전 정복 ⭐⭐⭐

### 1교시: Day 3 복습 + 함수 시작

- **복습 퀴즈 (10min)**: 제어문 전체, 리스트 컴프리헨션
- **핵심 복습 (15min)**: 
  - for문 복습 (enumerate, items)
  - 리스트 컴프리헨션 복습
  - 간단한 Q&A
- **함수 기본 시작 (25min)**:
  - 개념 (8min): 함수 필요성, FastAPI 엔드포인트와의 관계
  - Basic (17min):
    - def 키워드
    - 함수 호출
    - return
    - 여러 개 반환 (튜플)

### 2교시: 함수 기본 ⭐⭐

- **Basic 완성 (18min)**:
  - return 심화
  - 함수 없이 vs 함수 있을 때 비교
  - 실전 예제
- **Practice (20min)**:
  - 계산 함수
  - 문자열 처리 함수
  - 여러 값 반환 함수
- **Exercise (12min)**:
  - 온도 변환 함수
  - 인사말 함수

### 3교시: 매개변수 - 위치와 기본값 ⭐⭐⭐

- **개념 (10min)**: 매개변수 vs 인수, 기본값
- **Basic (20min)**:
  - 위치 인수
  - 기본값 (숫자, 문자열)
  - 조합
- **Practice (12min)**:
  - 인사 함수 (기본값 활용)
  - 프로필 출력
- **Exercise (8min)**:
  - 등급 계산 (기본값 활용)

### 4교시: 키워드 인수 + None 처리 ⭐⭐⭐

- **개념 (10min)**: 키워드 인수, None의 활용, FastAPI 쿼리 파라미터와의 관계
- **Basic (22min)**:
  - 키워드 인수
  - **None 기본값 패턴** (중요!):

    ```python
    def get_user(user_id: int, default=None):
        # None으로 "값 없음"을 표현
        if user_not_found:
            return default

    def create_profile(name: str, bio: str = None):
        # 선택적 매개변수
        if bio is None:
            bio = "소개가 없습니다"
    ```

  - 혼합 사용

- **Practice (10min)**:
  - API 스타일 함수
  - None 처리 연습
- **Exercise (8min)**:
  - 사용자 생성 함수 (None 활용)

### 5교시: 가변 인수 + 언패킹 통합 ⭐⭐⭐

- **개념 (10min)**: \*args, \*\*kwargs, 언패킹, FastAPI 핵심
- **Basic (22min)**:
  - \*args (여러 개 인수)
  - \*\*kwargs (키워드 인수들)
  - **딕셔너리 언패킹** `**dict`
  - **리스트 언패킹** `*list`
  - 조합 및 활용
  - 함수 호출 시 언패킹
- **Practice (10min)**:
  - 합계 함수 (\*args)
  - 로그 함수 (\*\*kwargs)
  - **설정 병합 (언패킹)**
- **Exercise (8min)**:
  - 유연한 계산기
  - 딕셔너리 병합 함수

### 6교시: 람다와 스코프 ⭐⭐

- **개념 (5min)**: 스코프, 람다
- **Basic (18min)**:
  - 지역/전역 변수
  - lambda
  - map/filter (간단히)
- **Practice (15min)**:
  - 변수 스코프 실험
  - 람다 활용
- **Exercise (12min)**:
  - 정렬 키
  - 간단한 변환

### 7교시: 예외 처리 ⭐⭐

- **개념 (8min)**: 예외 처리, FastAPI HTTPException 미리보기
- **Basic (20min)**:
  - try-except 기본
  - Exception as e
  - finally
  - raise
- **Practice (12min)**:
  - 안전한 입력
  - 검증
- **Exercise (10min)**:
  - 나누기 함수 (0 체크)
  - 파일 읽기 (에러 처리)

### 8교시: Day 4 종합 실습

- **복습 퀴즈 (10min)**: 함수 전체, 언패킹
- **🟢 기초 Problem (15min)**: 계산기 함수 모음 (\*args 활용)
- **🟡 응용 Problem (15min)**: 데이터 검증 시스템 (\*\*kwargs + 언패킹)
- **🔴 도전 Problem (10min)**: 유연한 API 함수 (None 처리 포함)

---

## Day 5: 클래스와 타입 힌트 ⭐⭐⭐

### 1교시: Day 4 복습 + 클래스 시작

- **복습 퀴즈 (10min)**: 함수, 가변 인수, None 처리, 언패킹
- **핵심 복습 (15min)**: 
  - \*args, \*\*kwargs 복습
  - 언패킹 복습
  - 간단한 Q&A
- **클래스 기본 시작 (25min)**:
  - 개념 (10min): OOP 개념, 클래스 vs 객체, Pydantic BaseModel 미리보기
  - Basic (15min):
    - class 정의
    - **init**
    - self
    - 인스턴스 생성

### 2교시: 클래스 기본 ⭐⭐

- **Basic 완성 (20min)**:
  - 메서드 추가
  - 속성 접근
  - 여러 인스턴스
  - 실전 예제
- **Practice (20min)**:
  - 학생 클래스
  - 계좌 클래스
  - 메서드 활용
- **Exercise (10min)**:
  - 상품 클래스
  - 복잡한 클래스

### 3교시: 클래스 상속 기초 ⭐⭐⭐

- **개념 (8min)**:
  - 상속이란? 코드 재사용
  - 부모 클래스, 자식 클래스
  - Pydantic BaseModel 미리보기
- **Basic (20min)**:
  - 간단한 상속 (10min):
    ```python
    class Animal:
        def speak(self):
            return "Some sound"
    
    class Dog(Animal):  # 상속!
        def speak(self):  # 오버라이딩!
            return "Woof!"
    ```
  - Pydantic 스타일 상속 (10min):
    ```python
    class UserBase(BaseModel):
        email: str
    
    class UserCreate(UserBase):
        password: str
    ```
- **Practice (15min)**:
  - 상품 → 할인상품 상속
  - BaseModel 상속 연습
  - 메서드 오버라이딩
- **Exercise (7min)**:
  - 직원 → 관리자 상속
  - Pydantic 모델 상속

> **중요**: super()는 제외! FastAPI에서 BaseModel 상속만 이해하면 충분!

### 4교시: 타입 힌트 (1) - 기본 ⭐⭐⭐

- **개념 (10min)**: 타입 힌트 필요성, FastAPI/Pydantic 핵심!
- **Basic (22min)**:
  - int, str, float, bool
  - 함수 타입 힌트 (매개변수, 반환값)
  - 타입 힌트는 "힌트"일 뿐 (강제 X)
  - 가독성 향상
- **Practice (10min)**:
  - 타입 힌트 추가 연습
- **Exercise (8min)**:
  - 기존 코드에 타입 추가

### 5교시: 타입 힌트 (2) - 고급 ⭐⭐⭐

- **개념 (10min)**: 복잡한 타입, Optional 중요성
- **Basic (20min)**:
  - List[int], Dict[str, int]
  - **Optional[str]** (핵심!)
  - Union[int, str]
  - 타입 힌트 조합
- **Practice (12min)**:
  - 복잡한 타입 작성
- **Exercise (8min)**:
  - API 응답 타입 (간단히)

### 6교시: 데코레이터 맛보기 + 함수 심화 실습 ⭐⭐

- **데코레이터 맛보기 (10min)**:
  - **개념 (5min)**: @ 문법, @app.get 미리보기
  - **간단한 언급 (5min)**:
    ```python
    # "이런 게 있다" 정도만
    @app.get("/users")
    def get_users():
        return {"users": []}
    
    # FastAPI에서 자연스럽게 쓰게 됨
    ```

- **함수 심화 실습 (40min)**:
  - \*args, \*\*kwargs 추가 연습 (15min)
  - None 처리 패턴 복습 (10min)
  - 타입 힌트 + 함수 조합 (10min)
  - Exercise: 복잡한 함수 작성 (5min)

### 7교시: import 완전 정복 ⭐⭐⭐

- **개념 (10min)**:
  - 모듈이란? 재사용 가능한 코드
  - 왜 필요? (FastAPI 프로젝트 구조)
  - 남의 코드 vs 내 코드
- **Basic (22min)**:
  - import 기본: `import json`
  - from import: `from json import dumps, loads`
  - 별칭: `import math as m`
  - 표준 라이브러리 (datetime, random)
  - **내 파일 import**:

    ```python
    # calculator.py
    def add(a, b):
        return a + b

    # main.py
    import calculator
    print(calculator.add(1, 2))
    ```

- **Practice (13min)**:
  - 계산기 모듈 만들기
  - 유틸리티 모듈
  - import하여 사용
- **Exercise (5min)**:
  - 검증 함수 모듈 작성

### 8교시: 기초 과정 종합 실습 ⭐⭐⭐

- **복습 퀴즈 (10min)**: Day 1-5 핵심 개념
- **🟢 기초 Problem (15min)**: 클래스 + 타입 힌트 시스템
- **🟡 응용 Problem (15min)**: 모듈화 프로젝트
- **🔴 도전 Problem (10min)**: 창의적 확장

---

## 📌 핵심 학습 목표 (FastAPI 중심)

### 최우선 항목 ⭐⭐⭐

1. **딕셔너리**: JSON의 기초, API 데이터 구조
2. **타입 힌트**: Pydantic 모델의 핵심
3. **함수 (매개변수, \*args, **kwargs, 언패킹)\*\*: 엔드포인트 작성
4. **클래스 (기초 + 상속)**: Pydantic BaseModel 이해
5. **None과 Optional**: 선택적 필드 처리
6. **데코레이터 개념**: @app.get 이해
7. **import**: 모듈화, FastAPI 프로젝트 구조
8. **리스트 컴프리헨션**: 데이터 변환
9. **문자열 (인덱싱, 슬라이싱, 메서드, f-string)**: API 데이터 처리
10. **for문**: 데이터 순회 및 처리

### 중요 항목 ⭐⭐

1. 리스트 (메서드, 내장 함수)
2. Boolean, Truthy/Falsy
3. 조건문 (if/elif/else)
4. 예외 처리
5. 튜플 (언패킹, 다중 리턴)

### 기본 항목 ⭐

1. 집합 (중복 제거, 빠른 검색)
2. while문
3. 람다 함수

---

## 📝 v9.0 주요 변경사항

1. ✅ **Day 1-1교시**: 환경 구축 50분 전체 확보
2. ✅ **Day 1 문자열**: 3교시로 확대 (기본 → 인덱싱/슬라이싱 → 메서드)
3. ✅ **Day 1-7교시**: 종합 실습 제거, 입출력+형변환으로 변경
4. ✅ **Day 3**: 중첩 딕셔너리 완전 제거
5. ✅ **Day 3-1~2교시**: Boolean을 Day 1에서 Day 3로 이동
6. ✅ **Day 3-4~5교시**: for문 2교시로 확대
7. ✅ v8.0 모든 개선사항 유지

---

## 🎯 학습 후 다음 단계

### 응용 과정 (Day 6-10)
- 웹과 API 이해
- FastAPI 시작
- Pydantic과 CRUD
- 데이터베이스 연동
- REST API 프로젝트

---
