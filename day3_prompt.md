# Day 3: 제어문 완전 정복

## Day 3: 제어문 완전 정복 - 01: Day 2 복습 + Boolean 시작

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`

### 📋 커리큘럼 내용
```
- **복습 퀴즈 (10분)**: 컬렉션 전체
- **핵심 복습 (15분)**: 
  - 딕셔너리 메서드 (items, get)
  - 리스트 vs 튜플 차이
  - 간단한 Q&A
- **Boolean + 비교 연산자 시작 (25분)**:
  - 개념 (10분): Boolean 타입, True/False, 조건 판단의 기초
  - Basic (15분):
    - True, False 값
    - 비교 연산자 (==, !=, <, >, <=, >=)
    - 간단한 조건 체크
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 02: Boolean + 비교 연산자

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_password_check.py`
4. `4_exercise_discount.py`
5. `solutions/solution_discount.py`
6. `solutions/solution_password_check.py`

### 📋 커리큘럼 내용
```
- **Basic 완성 (20분)**:
  - 논리 연산자 (and, or, not)
  - 조합 예제
  - 실전 패턴
- **Practice (20분)**:
  - 나이 비교 (성인인지 확인)
  - 로그인 검증 (아이디 and 비밀번호)
  - 범위 체크 (0 <= 점수 <= 100)
- **Exercise (10분)**:
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
3. `3_exercise_grade.py`
4. `4_exercise_login.py`
5. `solutions/solution_grade.py`
6. `solutions/solution_login.py`

### 📋 커리큘럼 내용
```
- **개념 (10분)**: 조건문 필요성, 논리 흐름
- **Basic (22분)**:
  - if/elif/else 기본
  - 논리 연산자 복습
  - Truthy/Falsy:
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

- **Practice (10분)**:
  - 성적 등급 (if/elif/else)
  - 로그인 검증
  - 빈 리스트 체크 (if items:)
- **Exercise (8분)**:
  - 할인율 계산
  - 안전한 데이터 접근 (if data:)
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 04: for문 기본

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_even_numbers.py`
4. `4_exercise_multiplication.py`
5. `solutions/solution_even_numbers.py`
6. `solutions/solution_multiplication.py`

### 📋 커리큘럼 내용
```
- **개념 (7분)**: 반복문, FastAPI 활용 (리스트 처리)
- **Basic (23분)**:
  - for 기본 문법
  - range() (1개, 2개, 3개 인자)
  - 리스트 순회
  - 간단한 예제
- **Practice (12분)**:
  - 리스트 출력
  - range() 활용
  - 합계 계산
- **Exercise (8분)**:
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
3. `3_exercise_enumerate.py`
4. `4_exercise_nested.py`
5. `solutions/solution_enumerate.py`
6. `solutions/solution_nested.py`

### 📋 커리큘럼 내용
```
- **개념 (5분)**: enumerate, items, 중첩 for문
- **Basic (22분)**:
  - enumerate() (인덱스 + 값)
  - items() (딕셔너리)
  - break/continue
  - 중첩 for문
- **Practice (13분)**:
  - 딕셔너리 순회
  - enumerate 활용
  - 중첩 for문 (구구단)
- **Exercise (10분)**:
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
3. `3_exercise_guess_number.py`
4. `4_exercise_menu.py`
5. `solutions/solution_guess_number.py`
6. `solutions/solution_menu.py`

### 📋 커리큘럼 내용
```
- **개념 (5분)**: while문, for vs while
- **Basic (18분)**:
  - while 기본
  - break/continue
  - 재시도 로직
- **Practice (15분)**:
  - 숫자 맞추기 게임
  - 메뉴 시스템
- **Exercise (12분)**:
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
3. `3_exercise_filter.py`
4. `4_exercise_transform.py`
5. `solutions/solution_filter.py`
6. `solutions/solution_transform.py`

### 📋 커리큘럼 내용
```
- **개념 (10분)**:
  - 왜 필요한가? 간결함, 성능
  - FastAPI에서 자주 사용
  - for문 vs 컴프리헨션 비교
  - 기본 패턴 이해
- **Basic (20분)**:
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
- **Practice (12분)**:
  - 짝수 리스트
  - 제곱 리스트
  - 필터링 + 변환
- **Exercise (8분)**:
  - 복잡한 변환
  - 딕셔너리 리스트 처리
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 3: 제어문 완전 정복 - 08: 종합 실습

### 📂 작성할 파일 목록
1. `1_basic_menu_system.py`
2. `2_intermediate_grade_processor.py`
3. `3_advanced_game.py`
4. `solutions/solution_game.py`
5. `solutions/solution_grade_processor.py`
6. `solutions/solution_menu_system.py`

### 📋 커리큘럼 내용
```
- **복습 퀴즈 (10분)**: Boolean, if문, for문, while문, 컴프리헨션
- **🟢 기초 Problem (15분)**: 메뉴 선택 (while + if)
- **🟡 응용 Problem (15분)**: 성적 처리 (for + 딕셔너리 + 컴프리헨션)
- **🔴 도전 Problem (10분)**: 간단한 게임 (종합)
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!