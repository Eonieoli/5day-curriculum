# Day 2: 컬렉션 자료형

## Day 2: 컬렉션 자료형 - 01: Day 1 복습 + 리스트 시작

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`

### 📋 커리큘럼 내용
```
- **복습 퀴즈 (10분)**: 변수, f-string, 문자열, 형변환
- **핵심 복습 (15분)**: 
  - f-string 실습
  - 문자열 메서드 복습
  - 간단한 Q&A
- **리스트 기본 시작 (25분)**:
  - 개념 (7분): 리스트란? 여러 값 저장, FastAPI 배열 처리
  - Basic (18분):
    - 리스트 생성 `[]`
    - 인덱싱 `[0]`, `[-1]`
    - 슬라이싱 `[start:end]`
    - 연산 (+, \*)
    - len() 함수
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 2: 컬렉션 자료형 - 02: 리스트 기본 + len()

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_scores.py`
4. `4_exercise_average.py`
5. `solutions/solution_average.py`
6. `solutions/solution_scores.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 2: 컬렉션 자료형 - 03: 리스트 수정

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_todo.py`
4. `4_exercise_inventory.py`
5. `solutions/solution_inventory.py`
6. `solutions/solution_todo.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 2: 컬렉션 자료형 - 04: 내장 함수 + 리스트 순수 함수

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_statistics.py`
4. `4_exercise_ranking.py`
5. `solutions/solution_ranking.py`
6. `solutions/solution_statistics.py`

### 📋 커리큘럼 내용
```
- **개념 (7분)**: 내장 함수란? 순수 함수 vs 메서드 차이
- **Basic (23분)**:
  - 핵심 내장 함수 (15분):
    - `len()`: 길이
    - `max()`, `min()`: 최댓값, 최솟값
    - `sum()`: 합계
    - `sorted()`: 정렬된 새 리스트 반환
  - 리스트 메서드 vs 순수 함수 (8분):
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 2: 컬렉션 자료형 - 05: 튜플 + 집합

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_coordinates.py`
4. `4_exercise_tags.py`
5. `solutions/solution_coordinates.py`
6. `solutions/solution_tags.py`

### 📋 커리큘럼 내용
```
- **튜플 (30분)**:
  - 개념 (7분): 튜플 불변성, 언패킹, 활용 사례
  - Basic (15분):
    - 튜플 생성 `()`, `tuple()`
    - 인덱싱 (리스트와 동일)
    - 언패킹 `x, y = (1, 2)`
    - 함수에서 여러 값 리턴
    - 수정 불가 특징
  - Practice (8분):
    - 좌표 처리 (x, y)
    - 함수 다중 리턴값
    - RGB 색상값
    - 여러 변수 동시 할당

- **집합 (20분)**:
  - 개념 (5분): 중복 제거, 빠른 검색 (O(1))
  - Basic (10분):
    - `set()` 생성
    - 중복 자동 제거
    - `in` 연산자로 검색
    - `add()`, `remove()`
  - Practice (3분):
    - 태그 중복 제거
    - 허용 사용자 목록 (set + in)
  - Exercise (2분):
    - 중복 제거 실습
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 2: 컬렉션 자료형 - 06: 딕셔너리 기초

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_student.py`
4. `4_exercise_profile.py`
5. `solutions/solution_profile.py`
6. `solutions/solution_student.py`

### 📋 커리큘럼 내용
```
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 2: 컬렉션 자료형 - 07: 딕셔너리 메서드

### 📂 작성할 파일 목록
1. `1_basic.py`
2. `2_practice.py`
3. `3_exercise_inventory.py`
4. `4_exercise_api_response.py`
5. `solutions/solution_api_response.py`
6. `solutions/solution_inventory.py`

### 📋 커리큘럼 내용
```
- **개념 (5분)**: get()의 중요성 (KeyError 방지)
- **Basic (22분)**:
  - `keys()`, `values()`, `items()`
  - `get(key, default)`
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
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!

---
## Day 2: 컬렉션 자료형 - 08: 종합 실습

### 📂 작성할 파일 목록
1. `1_basic_student_manager.py`
2. `2_intermediate_product_inventory.py`
3. `3_advanced_data_transform.py`
4. `solutions/solution_data_transform.py`
5. `solutions/solution_product_inventory.py`
6. `solutions/solution_student_manager.py`

### 📋 커리큘럼 내용
```
- **복습 퀴즈 (10분)**: 리스트, 튜플, 집합, 딕셔너리
- **🟢 기초 Problem (15분)**: 학생 관리 (딕셔너리)
- **🟡 응용 Problem (15분)**: 상품 재고 관리 (딕셔너리 + 리스트)
- **🔴 도전 Problem (10분)**: 데이터 변환 및 통계
```

### ✅ 작업 요청
위 파일들을 **코드 작성 규칙**과 **코드 형식 예시**에 따라 작성해주세요!