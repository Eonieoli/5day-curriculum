# Python 기초 과정 커리큘럼 v10

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
- **개념 완전 정복**: 25분 (새로운 주제의 순수 이론)

**실습 교시 (Day 2부터 매일 2교시, 50분)**

- **Basic**: 20-25분 (강사 시연)
- **Practice**: 15-20분 (함께 따라하기)
- **Exercise**: 7-12분 (스스로 풀기)

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
- **Git 설치 확인 (5분)**:
  - Git 버전 확인 (`git --version`)
  - 설치 안 된 학생 개별 지도
  - 지금은 버전 관리가 아니라 리눅스 명령어 사용을 위함을 설명
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

### 1교시: Day 1 복습 + 리스트 개념 완전 정복 ⭐⭐⭐

- **복습 퀴즈 (10분)**: 변수, f-string, 문자열, 형변환
- **핵심 복습 (15분)**:
  - f-string 실습 (가장 중요!)
  - 문자열 메서드 복습
  - 간단한 Q&A

- **리스트 개념 완전 정복 (25분)**:
  - **리스트란?** (7분):
    - 여러 값을 순서대로 저장하는 자료구조
    - 왜 필요한가? (변수 100개 vs 리스트 1개)
    - FastAPI에서 배열 데이터 처리
  - **인덱싱과 슬라이싱 개념** (8분):
    - 문자열과 동일한 방식
    - [0], [-1], [start:end]
    - 인덱스로 특정 요소 접근
  - **len() 함수의 역할** (5분):
    - 리스트 길이 확인
    - 반복문과의 관계 (미리보기)
  - **리스트 연산** (5분):
    - - 연산자로 리스트 합치기
    - - 연산자로 리스트 반복

> **중요**: 1교시는 순수 개념! 코드는 2교시에서!

### 2교시: 리스트 기본 + len() ⭐⭐

- **Basic (25분)**:
  - 리스트 생성 `[]`
  - 인덱싱 `[0]`, `[-1]`
  - 슬라이싱 `[start:end]`
  - 연산 (+, \*)
  - len() 함수 활용
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
- **Exercise (8min)**:
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
  - **Practice (3min)**:
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
  - 없는 key 접근 → KeyError 발생!
- **Practice (12분)**:
  - 학생 정보 딕셔너리
  - 상품 데이터
- **Exercise (8분)**:
  - 사용자 프로필 만들기

### 7교시: 딕셔너리 메서드 ⭐⭐⭐

- **개념 (5분)**: get()의 중요성 (KeyError 방지)
- **Basic (22min)**:
  - `keys()`, `values()`, `items()`
  - `get(key, default)` (핵심!)
  - `pop(key)`
  - `update()`
  - `in` 연산자 (if문 없이 간단히)
- **Practice (13min)**:
  - 딕셔너리 순회 (items())
  - 안전한 접근 (get())
  - 여러 딕셔너리 병합
- **Exercise (10min)**:
  - 상품 재고 관리
  - API 응답 처리 (딕셔너리 조합)

### 8교시: Day 2 종합 실습

- **복습 퀴즈 (10분)**: 리스트, 튜플, 집합, 딕셔너리
- **🟢 기초 Problem (15분)**: 학생 관리 (딕셔너리)
- **🟡 응용 Problem (15분)**: 상품 재고 관리 (딕셔너리 + 리스트)
- **🔴 도전 Problem (10분)**: 데이터 변환 및 통계

---

## Day 3: 제어문 완전 정복

### 1교시: Day 2 복습 + Boolean 개념 완전 정복 ⭐⭐⭐

- **복습 퀴즈 (10분)**: 컬렉션 전체
- **핵심 복습 (15분)**:
  - 딕셔너리 메서드 (items, get)
  - 리스트 vs 튜플 차이
  - 간단한 Q&A

- **Boolean + 비교 연산자 개념 완전 정복 (25분)**:
  - **Boolean 타입** (8분):
    - True/False란?
    - 조건 판단의 기초
    - 왜 필요한가? (프로그램의 분기)
    - 실생활 예시 (로그인 검증, 나이 확인)
  - **비교 연산자** (8분):
    - ==, !=, <, >, <=, >= 의미
    - 숫자 비교, 문자열 비교
    - 조건 체크의 핵심
  - **논리 연산자** (9분):
    - and: 둘 다 True
    - or: 하나만 True
    - not: 반대
    - 복잡한 조건 조합

> **중요**: 1교시는 순수 개념! 코드는 2교시에서!

### 2교시: Boolean + 비교 연산자 완성 ⭐⭐⭐

- **Basic (20min)**:
  - True, False 값 코드
  - 비교 연산자 실습
  - 논리 연산자 조합 예제
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

## Day 4: 함수와 타입 힌트 완전 정복 ⭐⭐⭐

### 1교시: Day 3 복습 + 함수 개념 완전 정복 ⭐⭐⭐

- **복습 퀴즈 (10min)**: 제어문 전체, 리스트 컴프리헨션
- **핵심 복습 (15min)**:
  - for문 복습 (enumerate, items)
  - 리스트 컴프리헨션 복습
  - 간단한 Q&A

- **함수 개념 완전 정복 (25min)**:
  - **함수란?** (8min):
    - 재사용 가능한 코드 블록
    - 왜 필요한가? (코드 중복 제거)
    - FastAPI 엔드포인트와의 관계
    - 입력 → 처리 → 출력
  - **매개변수와 반환값** (10min):
    - 매개변수: 함수의 입력
    - return: 함수의 출력
    - 여러 개 반환 (튜플)
    - 반환값 없는 함수 (None)
  - **함수 설계 원칙** (7min):
    - 하나의 함수는 하나의 역할
    - 명확한 이름 짓기
    - 적절한 매개변수 개수

> **중요**: 1교시는 순수 개념! 코드는 2교시에서!

### 2교시: 함수 기본 ⭐⭐

- **Basic (25min)**:
  - def 키워드
  - 함수 호출
  - return 심화
  - 여러 개 반환 (튜플)
  - 함수 없이 vs 함수 있을 때 비교
  - 실전 예제
- **Practice (15min)**:
  - 계산 함수
  - 문자열 처리 함수
  - 여러 값 반환 함수
- **Exercise (10min)**:
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

### 6교시: 타입 힌트 (1) - 기본 타입 ⭐⭐⭐

- **개념 (10min)**:
  - 타입 힌트 필요성
  - **FastAPI/Pydantic 핵심!**
  - 왜 함수에 타입이 필요?
  - 현대 Python의 표준
  - 타입 힌트는 "힌트"일 뿐 (강제 X)

- **Basic (22min)**:

  ```python
  # 기본 타입
  def add(a: int, b: int) -> int:
      return a + b

  def greet(name: str) -> str:
      return f"Hello, {name}"

  def calculate(price: float, tax: float = 0.1) -> float:
      return price * (1 + tax)

  def is_adult(age: int) -> bool:
      return age >= 18

  # 타입 힌트는 실행에 영향 없음
  result = add(1, 2)        # OK
  result = add("1", "2")    # 타입 에러지만 실행은 됨!

  # 가독성과 IDE 지원이 목적
  def process_data(data: str, count: int) -> str:
      return data * count
  ```

- **Practice (10min)**:
  - 기존 함수에 기본 타입 힌트 추가
  - 매개변수 타입 지정
  - 반환 타입 지정
- **Exercise (8min)**:
  - 타입 힌트가 있는 계산기 함수 작성
  - 여러 기본 타입 조합

> **중요**: 람다 삭제, 타입 힌트로 대체!
> 다음 교시에서 List, Dict, Optional 배움!

### 7교시: 타입 힌트 (2) - 고급 타입 ⭐⭐⭐

- **typing import 미리보기 (5min)**:
  - "내일 import를 자세히 배우지만, 오늘은 일단 따라 쓰세요"
  - `from typing import List, Dict, Optional, Union`
  - "typing이라는 모듈에서 타입 도구들을 가져오는 거예요"
  - "Python에 내장되어 있어서 설치 안 해도 됩니다"

- **개념 (5min)**:
  - 복잡한 타입의 필요성
  - FastAPI에서의 활용

- **Basic (24min)**:

  ```python
  from typing import List, Dict, Optional, Union

  # List 타입 (8min)
  def sum_list(numbers: List[int]) -> int:
      return sum(numbers)

  def process_names(names: List[str]) -> List[str]:
      return [name.upper() for name in names]

  # Dict 타입 (8min)
  def get_user_info() -> Dict[str, str]:
      return {"name": "Alice", "email": "alice@example.com"}

  def count_items(items: List[str]) -> Dict[str, int]:
      return {item: items.count(item) for item in set(items)}

  # Optional 타입 (중요!) (8min)
  def get_user(user_id: int) -> Optional[Dict[str, str]]:
      # None을 반환할 수 있음!
      if user_id == 1:
          return {"name": "Alice"}
      return None

  def find_item(items: List[str], target: str) -> Optional[str]:
      return target if target in items else None

  # Union 타입 (간단히)
  def process(value: Union[int, str]) -> str:
      return str(value)

  # *args, **kwargs에 타입!
  def add_all(*args: int) -> int:
      return sum(args)

  def create_user(**kwargs: str) -> Dict[str, str]:
      return kwargs
  ```

- **Practice (10min)**:
  - List, Dict 타입 힌트 추가
  - Optional 활용 (None 반환 함수)
  - 복잡한 타입 조합
- **Exercise (6min)**:
  - 타입 힌트가 완벽한 데이터 처리 함수
  - Optional을 활용한 검색 함수

> **중요**: Day 4에서 타입 힌트 100분 확보!
> FastAPI 준비 완료!

### 8교시: Day 4 종합 실습

- **복습 퀴즈 (10min)**: 함수 전체, 타입 힌트
- **🟢 기초 Problem (15min)**: 타입 힌트가 있는 계산기 함수 모음
- **🟡 응용 Problem (15min)**: List, Dict, Optional 활용 데이터 처리
- **🔴 도전 Problem (10min)**: \*args, \*\*kwargs + 완벽한 타입 힌트

---

## Day 5: 클래스 + 예외처리 + 모듈 ⭐⭐⭐

### 1교시: Day 4 복습 + 클래스 개념 완전 정복 ⭐⭐⭐

- **복습 퀴즈 (10min)**: 함수, 타입 힌트 전체
- **핵심 복습 (15min)**:
  - 타입 힌트 복습 (중요!)
  - Optional, List, Dict 복습
  - 간단한 Q&A

- **클래스 개념 완전 정복 (25min)**:
  - **객체지향 프로그래밍 (OOP)** (10min):
    - 클래스 vs 객체
    - 왜 필요한가? (데이터 + 기능 묶기)
    - 실생활 비유 (붕어빵 틀 vs 붕어빵)
    - Pydantic BaseModel 미리보기
  - **클래스 구조** (10min):
    - class 키워드
    - \***\*init\*\*** 메서드 (생성자)
    - self의 의미
    - 인스턴스 변수
    - 메서드 (함수와의 차이)
  - **타입 힌트와 클래스** (5min):
    - **init**에 타입 힌트
    - 메서드 반환 타입
    - FastAPI에서의 활용

> **중요**: 1교시는 순수 개념! 코드는 2교시에서!

### 2교시: 클래스 기본 ⭐⭐

- **Basic (25min)**:

  ```python
  class User:
      def __init__(self, name: str, age: int):
          self.name = name
          self.age = age

      def greet(self) -> str:
          return f"Hello, {self.name}"
  ```

  - 메서드 추가 (타입 힌트!)
  - 속성 접근
  - 여러 인스턴스
  - 실전 예제

- **Practice (15min)**:
  - 학생 클래스 (타입 힌트!)
  - 계좌 클래스 (타입 힌트!)
  - 메서드 활용
- **Exercise (10min)**:
  - 상품 클래스
  - 복잡한 클래스

### 3교시: 클래스 심화 ⭐⭐

- **Basic (20min)**:
  - 여러 메서드 (타입 힌트!)
  - 실전 패턴
  - 인스턴스 변수 vs 클래스 변수 (간단히)
- **Practice (20min)**:
  - 장바구니 클래스
  - TODO 리스트 클래스
  - 타입 힌트 완벽 적용
- **Exercise (10min)**:
  - 복잡한 클래스 설계

### 4교시: 클래스 상속 기초 ⭐⭐⭐

- **개념 (8min)**:
  - 상속이란? 코드 재사용
  - 부모 클래스, 자식 클래스
  - Pydantic BaseModel 미리보기
- **Basic (20min)**:
  - 간단한 상속 (10min):

    ```python
    class Animal:
        def __init__(self, name: str):
            self.name = name

        def speak(self) -> str:
            return "Some sound"

    class Dog(Animal):  # 상속!
        def speak(self) -> str:  # 오버라이딩!
            return "Woof!"
    ```

  - Pydantic 스타일 상속 (10min):

    ```python
    # FastAPI에서 이렇게 쓰게 됨!
    from pydantic import BaseModel

    class UserBase(BaseModel):
        email: str

    class UserCreate(UserBase):
        password: str

    class UserResponse(UserBase):
        id: int
    ```

- **Practice (15min)**:
  - 상품 → 할인상품 상속
  - BaseModel 상속 연습
  - 메서드 오버라이딩
- **Exercise (7min)**:
  - 직원 → 관리자 상속
  - Pydantic 모델 상속

> **중요**: super()는 제외! FastAPI에서 BaseModel 상속만 이해하면 충분!

### 5교시: 예외 처리 ⭐⭐

- **개념 (8min)**:
  - 예외 처리란?
  - 왜 필요한가?
  - FastAPI HTTPException 미리보기

- **Basic (20min)**:

  ```python
  # 기본 try-except
  def divide(a: int, b: int) -> float:
      try:
          return a / b
      except ZeroDivisionError:
          print("0으로 나눌 수 없습니다")
          return 0.0

  # Exception as e
  def process_data(data: str) -> int:
      try:
          return int(data)
      except ValueError as e:
          print(f"변환 실패: {e}")
          return 0

  # finally
  def read_file(filename: str) -> str:
      try:
          f = open(filename, 'r')
          return f.read()
      except FileNotFoundError:
          return "파일 없음"
      finally:
          f.close()  # 항상 실행!

  # raise
  def validate_age(age: int) -> None:
      if age < 0:
          raise ValueError("나이는 0 이상이어야 합니다")

  # 클래스 메서드에서 예외 처리
  class BankAccount:
      def __init__(self, balance: int):
          self.balance = balance

      def withdraw(self, amount: int) -> None:
          if amount > self.balance:
              raise ValueError("잔액 부족")
          self.balance -= amount
  ```

- **Practice (12min)**:
  - 안전한 입력 처리
  - 파일 읽기 예외 처리
  - 클래스 메서드 예외 처리
- **Exercise (10min)**:
  - 검증 함수 (예외 발생)
  - 안전한 클래스 메서드

### 6교시: 스코프 + 데코레이터 개념 ⭐⭐

- **스코프 (20min)**:
  - 개념 (5min):
    - 지역 변수 vs 전역 변수
    - 변수 스코프 규칙
  - Basic (10min):

    ```python
    # 지역 변수
    def func():
        x = 10  # 지역 변수
        return x

    # 전역 변수
    count = 0

    def increment():
        global count  # 전역 변수 사용
        count += 1

    # 클래스와 스코프
    class Counter:
        total = 0  # 클래스 변수

        def __init__(self):
            self.count = 0  # 인스턴스 변수
    ```

  - Practice (5min):
    - 변수 스코프 실험
    - 클래스 변수 vs 인스턴스 변수

- **데코레이터 개념 (30min)**:
  - 개념 (10min):
    - @ 문법이란?
    - **FastAPI에서 왜 @app.get("/users")?**
    - 함수를 꾸며주는 함수
  - Basic (15min):

    ```python
    # 간단한 데코레이터 이해
    def my_decorator(func):
        def wrapper():
            print("Before")
            func()
            print("After")
        return wrapper

    @my_decorator
    def say_hello():
        print("Hello!")

    # FastAPI에서는...
    @app.get("/users")  # ← 이게 데코레이터!
    def get_users():
        return {"users": []}

    # @property (간단히)
    class User:
        def __init__(self, name: str):
            self._name = name

        @property
        def name(self) -> str:
            return self._name
    ```

  - Practice (5min):
    - 데코레이터 이해
    - @app.get 패턴 이해

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
  - **typing import (복습!)** (중요!):
    ```python
    # 어제 써봤죠? 오늘 자세히 설명할게요!
    from typing import List, Dict, Optional, Union
    ```
  - **내 파일 import**:

    ```python
    # models.py
    from typing import Optional

    class User:
        def __init__(self, name: str, email: Optional[str] = None):
            self.name = name
            self.email = email

    # utils.py
    def validate_email(email: str) -> bool:
        return '@' in email

    # main.py
    from models import User
    from utils import validate_email

    user = User("Alice", "alice@example.com")
    if validate_email(user.email):
        print("Valid!")
    ```

- **Practice (13min)**:
  - 모델 모듈 만들기 (클래스 + 타입 힌트)
  - 유틸리티 모듈
  - import하여 사용
- **Exercise (5min)**:
  - 검증 함수 모듈 작성
  - 여러 모듈 조합

### 8교시: 기초 과정 종합 실습 ⭐⭐⭐

- **복습 퀴즈 (10min)**: Day 1-5 핵심 개념
- **🟢 기초 Problem (15min)**:
  - 타입 힌트가 완벽한 클래스 시스템
  - 여러 클래스 상속 구조
  - 예외 처리 포함
- **🟡 응용 Problem (15min)**:
  - 모듈화 프로젝트
  - models.py + utils.py + main.py 구조
  - 타입 힌트 완벽 적용
  - 예외 처리 강화
- **🔴 도전 Problem (10min)**:
  - FastAPI 스타일 모델 구조
  - BaseModel 상속 미리보기
  - 완전한 타입 시스템

---

## 📌 핵심 학습 목표 (FastAPI 중심)

### 최우선 항목 ⭐⭐⭐

1. **딕셔너리**: JSON의 기초, API 데이터 구조
2. **타입 힌트**: Pydantic 모델의 핵심 (Day 4에서 100분!)
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
4. 예외 처리 (Day 5로 이동!)
5. 튜플 (언패킹, 다중 리턴)
6. 스코프

### 기본 항목 ⭐

1. 집합 (중복 제거, 빠른 검색)
2. while문

---

## 🎯 학습 후 다음 단계

### 응용 과정 (Day 6-10)

- 웹과 API 이해
- FastAPI 시작
- Pydantic과 CRUD
- 데이터베이스 연동
- REST API 프로젝트
