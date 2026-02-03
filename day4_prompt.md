# Day 4: 함수와 타입 힌트

## Day 4: 함수와 타입 힌트 - 01_02: 함수 기본

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 4: 함수와 타입 힌트 - 03: 매개변수 - 위치와 기본값

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 4: 함수와 타입 힌트 - 04: 키워드 인수 + None 처리

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 4: 함수와 타입 힌트 - 05: 가변 인수 + 언패킹

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 4: 함수와 타입 힌트 - 06: 타입 힌트 (1) - 기본 타입

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 4: 함수와 타입 힌트 - 07: 타입 힌트 (2) - 고급 타입

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise.py`
4. `3_exercise_solution.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 4: 함수와 타입 힌트 - 08: 종합 실습

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_intermediate.py`
3. `3_advanced.py`
4. `1_basic_solution.py`
5. `2_intermediate_solution.py`
6. `3_advanced_solution.py`

### 📋 커리큘럼 내용
```
### 8교시: Day 4 종합 실습

- **복습 퀴즈 (10min)**: 함수 전체, 타입 힌트
- **🟢 기초 Problem (15min)**: 타입 힌트가 있는 계산기 함수 모음
- **🟡 응용 Problem (15min)**: List, Dict, Optional 활용 데이터 처리
- **🔴 도전 Problem (10min)**: \*args, \*\*kwargs + 완벽한 타입 힌트
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!