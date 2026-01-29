# Day 5: 클래스 + 예외처리 + 모듈

## Day 5: 클래스 + 예외처리 + 모듈 - 01: Day 4 복습 + 클래스 시작

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`

### 📋 커리큘럼 내용
```
- **복습 퀴즈 (10분)**: 함수, 타입 힌트 전체
- **핵심 복습 (15분)**: 
  - 타입 힌트 복습
  - Optional, List, Dict 복습
  - 간단한 Q&A
- **클래스 기본 시작 (25분)**:
  - 개념 (10분): OOP 개념, 클래스 vs 객체, Pydantic BaseModel 미리보기
  - Basic (15분):
    - class 정의
    - __init__ (타입 힌트와 함께)
    - self
    - 인스턴스 생성
    ```python
    class User:
        def __init__(self, name: str, age: int):
            self.name = name
            self.age = age
        
        def greet(self) -> str:
            return f"Hello, {self.name}"
    ```
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 02: 클래스 기본

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_student.py`
4. `4_exercise_account.py`
5. `solutions/solution_account.py`
6. `solutions/solution_student.py`

### 📋 커리큘럼 내용
```
- **Basic 완성 (20분)**:
  - 메서드 추가 (타입 힌트)
  - 속성 접근
  - 여러 인스턴스
  - 실전 예제
- **Practice (20분)**:
  - 학생 클래스 (타입 힌트)
  - 계좌 클래스 (타입 힌트)
  - 메서드 활용
- **Exercise (10분)**:
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
3. `3_exercise_cart.py`
4. `4_exercise_todo.py`
5. `solutions/solution_cart.py`
6. `solutions/solution_todo.py`

### 📋 커리큘럼 내용
```
- **Basic (20분)**:
  - 여러 메서드 (타입 힌트)
  - 실전 패턴
  - 인스턴스 변수 vs 클래스 변수
- **Practice (20분)**:
  - 장바구니 클래스
  - TODO 리스트 클래스
  - 타입 힌트 완벽 적용
- **Exercise (10분)**:
  - 복잡한 클래스 설계
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 04: 클래스 상속

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_product.py`
4. `4_exercise_employee.py`
5. `solutions/solution_employee.py`
6. `solutions/solution_product.py`

### 📋 커리큘럼 내용
```
- **개념 (8분)**:
  - 상속이란? 코드 재사용
  - 부모 클래스, 자식 클래스
  - Pydantic BaseModel 미리보기
- **Basic (20분)**:
  - 간단한 상속:
    ```python
    class Animal:
        def __init__(self, name: str):
            self.name = name
        
        def speak(self) -> str:
            return "Some sound"
    
    class Dog(Animal):  # 상속
        def speak(self) -> str:  # 오버라이딩
            return "Woof!"
    ```
  - Pydantic 스타일 상속:
    ```python
    from pydantic import BaseModel
    
    class UserBase(BaseModel):
        email: str
    
    class UserCreate(UserBase):
        password: str
    
    class UserResponse(UserBase):
        id: int
    ```
- **Practice (15분)**:
  - 상품 → 할인상품 상속
  - BaseModel 상속 연습
  - 메서드 오버라이딩
- **Exercise (7분)**:
  - 직원 → 관리자 상속
  - Pydantic 모델 상속
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 05: 예외 처리

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_safe_input.py`
4. `4_exercise_validator.py`
5. `solutions/solution_safe_input.py`
6. `solutions/solution_validator.py`

### 📋 커리큘럼 내용
```
- **개념 (8분)**:
  - 예외 처리란?
  - 왜 필요한가?
  - FastAPI HTTPException 미리보기

- **Basic (20분)**:
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
          f.close()  # 항상 실행
  
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

- **Practice (12분)**:
  - 안전한 입력 처리
  - 파일 읽기 예외 처리
  - 클래스 메서드 예외 처리
  
- **Exercise (10분)**:
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
3. `3_exercise_scope.py`
4. `solutions/solution_scope.py`

### 📋 커리큘럼 내용
```
- **스코프 (20분)**:
  - 개념 (5분):
    - 지역 변수 vs 전역 변수
    - 변수 스코프 규칙
  - Basic (10분):
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
  - Practice (5분):
    - 변수 스코프 실험
    - 클래스 변수 vs 인스턴스 변수

- **데코레이터 개념 (30분)**:
  - 개념 (10분):
    - @ 문법이란?
    - FastAPI에서 왜 @app.get("/users")?
    - 함수를 꾸며주는 함수
  - Basic (15분):
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
    @app.get("/users")  # ← 이게 데코레이터
    def get_users():
        return {"users": []}
    
    # @property
    class User:
        def __init__(self, name: str):
            self._name = name
        
        @property
        def name(self) -> str:
            return self._name
    ```
  - Practice (5분):
    - 데코레이터 이해
    - @app.get 패턴 이해
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 5: 클래스 + 예외처리 + 모듈 - 07: import 완전 정복

### 📂 작성할 파일 목록
1. `1_basic_example/main.py`
2. `1_basic_example/models.py`
3. `1_basic_example/utils.py`
4. `2_practice_project/main.py`
5. `2_practice_project/calculator.py`
6. `2_practice_project/student.py`
7. `3_exercise_project/main.py`
8. `3_exercise_project/models.py`
9. `3_exercise_project/utils.py`
10. `solutions/solution_main.py`
11. `solutions/solution_models.py`
12. `solutions/solution_utils.py`

### 📋 커리큘럼 내용
```
- **개념 (10분)**:
  - 모듈이란? 재사용 가능한 코드
  - 왜 필요? (FastAPI 프로젝트 구조)
  - 남의 코드 vs 내 코드
  
- **Basic (22분)**:
  - import 기본: `import json`
  - from import: `from json import dumps, loads`
  - 별칭: `import math as m`
  - 표준 라이브러리 (datetime, random)
  - typing import:
    ```python
    from typing import List, Dict, Optional, Union
    ```
  - 내 파일 import:
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

- **Practice (13분)**:
  - 모델 모듈 만들기 (클래스 + 타입 힌트)
  - 유틸리티 모듈
  - import하여 사용
  
- **Exercise (5분)**:
  - 검증 함수 모듈 작성
  - 여러 모듈 조합
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---

## Day 5: 클래스 + 예외처리 + 모듈 - 08: 종합 실습

### 📂 작성할 파일 목록
1. `1_basic_class_system.py`
2. `2_intermediate_modular_app.py`
3. `3_advanced_complete.py`
4. `solutions/solution_class_system.py`
5. `solutions/solution_complete.py`
6. `solutions/solution_modular_app.py`

### 📋 커리큘럼 내용
```
- **복습 퀴즈 (10분)**: Day 1-5 핵심 개념
- **🟢 기초 Problem (15분)**: 
  - 타입 힌트가 완벽한 클래스 시스템
  - 여러 클래스 상속 구조
  - 예외 처리 포함
- **🟡 응용 Problem (15분)**: 
  - 모듈화 프로젝트
  - models.py + utils.py + main.py 구조
  - 타입 힌트 완벽 적용
  - 예외 처리 강화
- **🔴 도전 Problem (10분)**: 
  - FastAPI 스타일 모델 구조
  - BaseModel 상속 미리보기
  - 완전한 타입 시스템
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!