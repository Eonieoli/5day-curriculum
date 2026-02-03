# Day 3: 제어문 완전 정복

## Day 3: 제어문 완전 정복 - 01_02: Boolean + 비교/논리 연산자

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
### 1교시: Day 2 복습 + Boolean 개념 완전 정복 ⭐⭐⭐

- **복습 퀴즈 (10분)**: 컬렉션 전체
- **핵심 복습 (15분)**:
  - 딕셔너리 메서드 (items, get)
  - 리스트 vs 튜플 차이
  - 간단한 Q&A

- **Boolean + 비교/논리 연산자 개념 완전 정복 (25분)**:
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

### 2교시: Boolean + 비교/논리 연산자 완성 ⭐⭐⭐

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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 03: 조건문 + Truthy/Falsy

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 04: for문 기본

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 05: for문 심화

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 06: while문

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 07: 리스트 컴프리헨션

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 08: 종합 실습

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_intermediate.py`
3. `3_advanced.py`
4. `1_basic_solution.py`
5. `2_intermediate_solution.py`
6. `3_advanced_solution.py`

### 📋 커리큘럼 내용
```
### 8교시: Day 3 종합 실습

- **복습 퀴즈 (10min)**: Boolean, if문, for문, while문, 컴프리헨션
- **🟢 기초 Problem (15min)**: 메뉴 선택 (while + if)
- **🟡 응용 Problem (15min)**: 성적 처리 (for + 딕셔너리 + 컴프리헨션)
- **🔴 도전 Problem (10min)**: 간단한 게임 (종합)
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!