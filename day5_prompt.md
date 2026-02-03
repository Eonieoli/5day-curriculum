# Day 5: 클래스 + 예외처리 + 모듈

## Day 5: 클래스 + 예외처리 + 모듈 - 01_02: 클래스 기본

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 03: 클래스 심화

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 04: 클래스 상속

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 05: 예외 처리

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 06: 스코프 + 데코레이터 개념

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 07: import 완전 정복

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---

## Day 5: 클래스 + 예외처리 + 모듈 - 08: 종합 실습

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_intermediate.py`
3. `3_advanced.py`
4. `1_basic_solution.py`
5. `2_intermediate_solution.py`
6. `3_advanced_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!