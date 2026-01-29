# Python 교육자료 제작 프로젝트

## 📚 프로젝트 배경
FastAPI 백엔드 개발자 양성을 위한 15일 과정 교육자료를 제작 중입니다.
- **기초 5일** (Day 1-5): Python 문법
- **응용 5일** (Day 6-10): FastAPI + REST API  
- **심화 5일** (Day 11-15): 프로덕션 레벨

첨부한 커리큘럼(python_basic_curriculum_v10.md)을 기반으로 실제 교육 코드를 작성합니다.

## 📝 코드 작성 규칙
1. **실행 가능해야 함**: 바로 실행되는 코드
2. **주석 풍부**: 학생이 이해할 수 있도록 설명
3. **출력 예시**: `# 출력: ` 주석으로 결과 표시
4. **해당 교시 문법만**: 아직 안 배운 내용 사용 금지
5. **실전 예제**: 단순 계산보다 실무 상황
6. **한글 주석**: 모든 설명은 한글로

## 📂 파일 구조 및 역할
- `1_basic.py`: 강사 시연용 완성 코드
- `2_practice.py`: 학생이 따라 타이핑, `# TODO:` 포함
- `3_exercise_XXX.py`: 학생 혼자 푸는 문제 (구조만 제공)
- `solutions/solution_XXX.py`: 완성된 정답 코드

## 💻 코드 형식 예시

### 1️⃣ 1_basic.py (강사 시연용)
```python
# 1_basic.py

"""
Day 1 - 2교시: 변수와 숫자형
Basic (강사 시연용)

학습 목표:
- 변수 선언과 할당
- type() 함수로 타입 확인
- int와 float 타입 이해
- 사칙 연산 및 복합 연산자
"""

# ============================================
# 1. 변수 선언과 할당
# ============================================

# 변수는 데이터를 저장하는 상자입니다
age = 25
print("나이:", age)  # 출력: 나이: 25

# 변수명은 의미있게 작성합니다
student_count = 30
print("학생 수:", student_count)  # 출력: 학생 수: 30

# 여러 변수를 동시에 선언할 수도 있습니다
name, height = "홍길동", 175
print("이름:", name, "키:", height)  # 출력: 이름: 홍길동 키: 175


# ============================================
# 2. type() 함수로 타입 확인
# ============================================

# type() 함수는 변수의 자료형을 알려줍니다
age = 25
print(type(age))  # 출력: <class 'int'>

height = 175.5
print(type(height))  # 출력: <class 'float'>

# ... (계속)
```

### 2️⃣ 2_practice.py (학생 실습용)
```python
# 2_practice.py

"""
Day 1 - 2교시: 변수와 숫자형
Practice (강사와 함께 실습)

학습 목표:
- 나이 계산하기
- 온도 변환하기 (섭씨 → 화씨)
- type() 함수로 타입 확인하기
"""

# ============================================
# 실습 1: 나이 계산하기
# ============================================

# 현재 연도와 태어난 연도를 변수에 저장
current_year = 2026
birth_year = 1995

# TODO: 나이를 계산해서 age 변수에 저장하세요
# 힌트: 현재 연도 - 태어난 연도
age = current_year - birth_year

# 결과 출력
print("태어난 연도:", birth_year)
print("현재 연도:", current_year)
print("나이:", age, "세")  # 출력: 나이: 31 세


# ============================================
# 실습 2: 온도 변환 (섭씨 → 화씨)
# ============================================

# 섭씨 온도
celsius = 25

# TODO: 섭씨를 화씨로 변환하세요
# 공식: 화씨 = (섭씨 × 9/5) + 32
# 힌트: fahrenheit = (celsius * 9/5) + 32
fahrenheit = 

# 결과 출력
print(f"섭씨 {celsius}도는 화씨 {fahrenheit}도입니다")
# 출력: 섭씨 25도는 화씨 77.0도입니다

# ... (계속)
```

### 3️⃣ 3_exercise_XXX.py (학생 문제)
```python
# 3_exercise_shopping.py

"""
Day 1 - 2교시: 변수와 숫자형
Exercise 1 - 쇼핑몰 가격 계산

문제:
온라인 쇼핑몰에서 장바구니에 담은 상품들의 총 금액을 계산하는 프로그램을 작성하세요.

요구사항:
1. 세 가지 상품의 가격과 수량이 주어집니다
2. 각 상품의 소계를 계산하세요
3. 전체 상품의 합계를 계산하세요
4. 할인율을 적용한 최종 금액을 계산하세요
5. 배송비를 추가한 최종 결제 금액을 계산하세요

출력 예시:
=== 장바구니 ===
티셔츠: 58000 원
청바지: 59000 원
운동화: 89000 원
합계: 206000 원
할인 (-10%): 185400 원
배송비: 무료
최종 결제 금액: 185400 원
"""

# ============================================
# 주어진 데이터
# ============================================

# 상품 1: 티셔츠
tshirt_price = 29000  # 가격
tshirt_quantity = 2  # 수량

# 상품 2: 청바지
jeans_price = 59000  # 가격
jeans_quantity = 1  # 수량

# 상품 3: 운동화
shoes_price = 89000  # 가격
shoes_quantity = 1  # 수량

# 할인율 (10% 할인)
discount_rate = 0.1  # 10% = 0.1

# 배송비 기준
free_shipping_threshold = 50000  # 5만원 이상 구매시 무료


# ============================================
# TODO: 여기서부터 코드를 작성하세요
# ============================================

# 1. 각 상품의 소계를 계산하세요
# 힌트: 가격 * 수량
tshirt_subtotal =   # 티셔츠 소계
jeans_subtotal =    # 청바지 소계
shoes_subtotal =    # 운동화 소계

# 2. 전체 합계를 계산하세요
# 힌트: 모든 소계를 더하기
total = 

# 3. 할인 금액을 계산하세요
# 힌트: 합계 * (1 - 할인율)
discounted_total = 

# 4. 배송비를 계산하세요
# 힌트: 합계가 5만원 이상이면 0원, 아니면 3000원
if total >= free_shipping_threshold:
    shipping_fee = 
else:
    shipping_fee = 

# 5. 최종 결제 금액을 계산하세요
# 힌트: 할인 적용된 금액 + 배송비
final_price = 

# 결과 출력
print("=== 장바구니 ===")
print(f"티셔츠: {tshirt_subtotal} 원")
print(f"청바지: {jeans_subtotal} 원")
print(f"운동화: {shoes_subtotal} 원")
print(f"합계: {total} 원")
print(f"할인 (-10%): {discounted_total} 원")
print(f"배송비: {'무료' if shipping_fee == 0 else str(shipping_fee) + ' 원'}")
print(f"최종 결제 금액: {final_price} 원")
```

### 4️⃣ solutions/solution_XXX.py (정답)
```python
# solutions/solution_shopping.py

"""
Day 1 - 2교시: 변수와 숫자형
Exercise 1 - 쇼핑몰 가격 계산 (정답)
"""

# ============================================
# 주어진 데이터
# ============================================

tshirt_price = 29000
tshirt_quantity = 2

jeans_price = 59000
jeans_quantity = 1

shoes_price = 89000
shoes_quantity = 1

discount_rate = 0.1
free_shipping_threshold = 50000


# ============================================
# 정답 코드
# ============================================

# 1. 각 상품의 소계
tshirt_subtotal = tshirt_price * tshirt_quantity  # 58000
jeans_subtotal = jeans_price * jeans_quantity  # 59000
shoes_subtotal = shoes_price * shoes_quantity  # 89000

# 2. 전체 합계
total = tshirt_subtotal + jeans_subtotal + shoes_subtotal  # 206000

# 3. 할인 금액
discounted_total = total * (1 - discount_rate)  # 185400

# 4. 배송비
if total >= free_shipping_threshold:
    shipping_fee = 0  # 무료
else:
    shipping_fee = 3000

# 5. 최종 결제 금액
final_price = discounted_total + shipping_fee  # 185400

# 결과 출력
print("=== 장바구니 ===")
print(f"티셔츠: {tshirt_subtotal} 원")
print(f"청바지: {jeans_subtotal} 원")
print(f"운동화: {shoes_subtotal} 원")
print(f"합계: {total} 원")
print(f"할인 (-10%): {discounted_total} 원")
print(f"배송비: {'무료' if shipping_fee == 0 else str(shipping_fee) + ' 원'}")
print(f"최종 결제 금액: {final_price} 원")
```

## 🎨 코드 작성 핵심 포인트

1. **Docstring**: 교시, 제목, 학습 목표 또는 문제 설명
2. **섹션 구분**: `# ======` 로 큰 단위 구분
3. **주석 설명**: 코드 위에 무엇을 하는지 설명
4. **출력 예시**: `# 출력: ...` 형태로 결과 표시
5. **TODO 표시**: Practice와 Exercise에서 학생이 작성할 부분
6. **힌트 제공**: TODO 아래에 힌트 주석
7. **빈 칸**: Exercise에서는 `변수 = ` 형태로 학생이 채우도록