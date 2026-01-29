# Python 기초 과정 커리큘럼 v3.0

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

**복습 교시 (매일 1교시, 50분)**
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

### 1교시: Python 첫걸음
- **개념 (10분)**: 오리엔테이션, Python 특징, 실행 방법
- **Basic (15분)**: print(), 주석, 간단한 계산
- **Practice (20분)**: 자기소개 출력, 계산 실습
- **Exercise (5분)**: 회사 정보 출력

### 2교시: 변수와 숫자형 + type() ⭐⭐
- **개념 (8분)**: 변수, int/float, type() 함수로 타입 확인
- **Basic (18분)**: 변수 선언, type() 확인, 사칙 연산, 복합 연산자
- **Practice (15분)**: 나이 계산, 온도 변환, type() 실습
- **Exercise (9분)**: 쇼핑몰 가격 계산

### 3교시: 문자열 기본 ⭐⭐
- **개념 (7분)**: 문자열, 인덱싱, 슬라이싱
- **Basic (18분)**: 문자열 생성/연산, 인덱싱, 슬라이싱
- **Practice (15분)**: 이메일 분리, 파일명 처리
- **Exercise (10분)**: 전화번호 포맷팅

### 4교시: f-string 완전 정복 ⭐⭐⭐
- **개념 (5분)**: 포매팅 필요성, f-string 사용 이유
- **Basic (25분)**: f-string 문법, 표현식, 포매팅 옵션, 정렬
- **Practice (15분)**: 상품 정보, 성적표, 로그 메시지
- **Exercise (5분)**: 회원 카드 출력

### 5교시: 문자열 메서드 + Boolean ⭐⭐
- **개념 (5분)**: 메서드 개념, Boolean, Truthy/Falsy 간단히 언급 (2분)
- **Basic (20분)**: upper/lower/strip, split/join, replace, Boolean, 비교 연산자
- **Practice (15분)**: 이메일 검증, 데이터 정제
- **Exercise (10분)**: 비밀번호 강도 체크

### 6교시: 입출력 + 형변환 ⭐⭐
- **개념 (7분)**: input() 특징, 형변환 필요성
- **Basic (18분)**: input(), int/str/float 형변환, 안전한 변환
- **Practice (15분)**: 계산기, BMI 계산기
- **Exercise (10분)**: 거스름돈 계산

### 7교시: 복습 + 연습 문제 ⭐⭐
- **개념 복습 (15분)**: Day 1 핵심 내용 빠른 정리
- **추가 연습 (25분)**: 학생들이 어려워한 부분 재실습
- **자유 실습 (10분)**: 자신만의 프로그램 만들어보기

### 8교시: Day 1 종합 실습
- **복습 퀴즈 (10분)**: Day 1 핵심 내용
- **🟢 기초 Problem (15분)**: 프로필 카드 생성기 (f-string 활용)
- **🟡 응용 Problem (15분)**: 쇼핑몰 영수증 (여러 개념 조합)
- **🔴 도전 Problem (10분)**: 스마트 계산기 (입력 검증 포함)

---

## Day 2: 컬렉션 자료형

### 1교시: Day 1 복습
- **퀴즈 (20분)**: 변수, f-string, Boolean, 형변환
- **실습 복습 (25분)**: 어제 Exercise 재도전
- **Q&A (5분)**

### 2교시: 리스트 기본 ⭐⭐
- **개념 (7분)**: 리스트 개념, FastAPI 배열 처리
- **Basic (18분)**: 생성, 인덱싱, 슬라이싱, 연산
- **Practice (15분)**: 학생 점수 관리, 슬라이싱 연습
- **Exercise (10분)**: 성적 처리

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
- **개념 (8분)**: 튜플 불변성, 집합 중복 제거
- **Basic - 튜플 (15분)**: 생성, 언패킹, 활용
- **Basic - 집합 (7분)**: set(), 중복 제거, in 연산 (빠른 검색)
- **Practice (15분)**: 좌표 처리(튜플), 중복 제거(집합)
- **Exercise (5분)**: 함수 리턴값(튜플), 유니크 데이터(집합)

### 6교시: 딕셔너리 개념 ⭐⭐⭐
- **개념 (10분)**: key-value, JSON 구조, FastAPI 핵심
- **Basic (22분)**: 생성, 접근, 추가/수정/삭제, in 연산자
- **Practice (13분)**: 학생 정보, 상품 재고
- **Exercise (5분)**: 연락처 관리

### 7교시: 딕셔너리 메서드 ⭐⭐⭐
- **개념 (5분)**: get()의 중요성
- **Basic (22분)**: keys/values/items, get, pop/update
- **Practice (15분)**: 딕셔너리 순회, 안전한 접근
- **Exercise (8분)**: API 응답 처리 (딕셔너리 조합)

### 8교시: Day 2 종합 실습
- **복습 퀴즈 (10분)**: 리스트, 튜플, 딕셔너리
- **🟢 기초 Problem (15분)**: 학생 관리 (딕셔너리)
- **🟡 응용 Problem (20분)**: 상품 재고 관리 (딕셔너리 + 리스트)
- **🔴 도전 Problem (5분)**: JSON 형식 변환 준비

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
- **Exercise (7분)**: 복잡한 JSON 처리

### 3교시: 딕셔너리 심화 (2) - 언패킹 ⭐⭐⭐
- **개념 (10분)**: 딕셔너리 언패킹, **kwargs 미리보기
- **Basic (22분)**: 언패킹 활용, 딕셔너리 병합
- **Practice (13분)**: 설정 데이터 병합
- **Exercise (5분)**: 여러 딕셔너리 합치기

### 4교시: 조건문 (if) + Truthy/Falsy ⭐⭐⭐
- **개념 (10분)**: 조건문 필요성, 논리 흐름, Truthy/Falsy 개념
- **Basic (22분)**: 
  - if/elif/else 기본
  - 논리 연산자 (and, or, not)
  - Truthy/Falsy 활용 (if name:, if items:, if not data:)
  - in 연산자
- **Practice (13분)**: 성적 등급, 로그인 검증, 안전한 조건문
- **Exercise (5분)**: 할인율 계산

### 5교시: for문 ⭐⭐⭐
- **개념 (7분)**: 반복문, FastAPI 활용
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
- **개념 (8분)**: 함수 필요성, FastAPI 엔드포인트
- **Basic (18분)**: def, 호출, return, 여러 개 반환
- **Practice (15분)**: 계산 함수, 문자열 처리
- **Exercise (9분)**: 온도 변환

### 3교시: 매개변수 (1) - 위치와 기본값 + None ⭐⭐⭐
- **개념 (10분)**: 매개변수 vs 인수, 기본값, None의 활용
- **Basic (22분)**: 
  - 위치 인수
  - 기본값 (숫자, 문자열)
  - None 기본값 패턴
  - 조합
- **Practice (13분)**: 인사 함수, 프로필 출력, None 처리
- **Exercise (5분)**: 등급 계산

### 4교시: 매개변수 (2) - 키워드 인수 ⭐⭐⭐
- **개념 (8분)**: 키워드 인수, FastAPI 쿼리 파라미터
- **Basic (20분)**: 키워드 인수, 혼합, 실전 예제
- **Practice (14분)**: API 스타일 함수
- **Exercise (8분)**: 사용자 생성

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

### 7교시: 예외 처리 ⭐⭐
- **개념 (8분)**: 예외 처리, FastAPI HTTPException
- **Basic (20분)**: try-except, Exception as e, finally, raise
- **Practice (15분)**: 안전한 입력, 검증
- **Exercise (7분)**: 나누기 함수

### 8교시: Day 4 종합 실습
- **복습 퀴즈 (10분)**: 함수 전체
- **🟢 기초 Problem (15분)**: 계산기 함수 모음 (*args 활용)
- **🟡 응용 Problem (20분)**: 데이터 검증 시스템 (**kwargs 활용)
- **🔴 도전 Problem (5분)**: 유연한 API 함수

---

## Day 5: 클래스와 타입 힌트 ⭐⭐⭐

### 1교시: Day 4 복습
- **퀴즈 (20분)**: 함수, 가변 인수, None 처리
- **실습 복습 (25분)**: *args, **kwargs 집중
- **Q&A (5분)**

### 2교시: 클래스 기본 ⭐⭐
- **개념 (10분)**: OOP 개념, 클래스 vs 객체
- **Basic (20분)**: class 정의, __init__, self, 인스턴스
- **Practice (13분)**: 학생 클래스, 계좌 클래스
- **Exercise (7분)**: 상품 클래스

### 3교시: 클래스 활용 + isinstance() ⭐⭐
- **개념 (7분)**: 인스턴스 메서드, isinstance() vs type()
- **Basic (20분)**: 메서드 작성, isinstance() 활용
- **Practice (15분)**: TODO 클래스, 타입 체크
- **Exercise (8분)**: 유저 클래스

### 4교시: 타입 힌트 (1) - 기본 ⭐⭐⭐
- **개념 (10분)**: 타입 힌트 필요성, FastAPI 핵심
- **Basic (22분)**: int, str, float, bool, 함수 타입 힌트
- **Practice (13분)**: 타입 힌트 추가
- **Exercise (5분)**: 기존 코드 타입 추가

### 5교시: 타입 힌트 (2) - 고급 ⭐⭐⭐
- **개념 (10분)**: 복잡한 타입, Optional 중요성
- **Basic (20분)**: List[int], Dict[str, int], Optional, Union
- **Practice (13분)**: 복잡한 타입 작성
- **Exercise (7분)**: API 응답 타입 (간단히)

### 6교시: 데코레이터 ⭐⭐
- **개념 (10분)**: 데코레이터 개념, @app.get 미리보기
- **Basic (20분)**: 데코레이터 기본, 간단한 예제
- **Practice (15분)**: 로깅 데코레이터
- **Exercise (5분)**: 타이머 데코레이터

### 7교시: import + JSON ⭐⭐⭐
- **개념 (10분)**:
  - import 기본 개념 (3분): 남의 코드 가져다 쓰기
  - import 문법 (2분): import json, from json import dumps
  - JSON이란? (5분): 딕셔너리 ↔ 텍스트, 왜 필요한가?

- **Basic (22분)**:
  - 딕셔너리 → JSON 문자열 (8분)
    - json.dumps(딕셔너리)
    - indent 옵션으로 예쁘게
  - JSON 문자열 → 딕셔너리 (6분)
    - json.loads(문자열)
  - 파일 저장/로드 (8분)
    - json.dump(딕셔너리, 파일)
    - json.load(파일)
    - with open() 패턴

- **Practice (13분)**:
  - 학생 정보 딕셔너리 만들기
  - JSON 파일로 저장
  - 파일에서 읽어오기
  - 수정 후 다시 저장

- **Exercise (5분)**:
  - 상품 목록을 JSON으로 관리하는 프로그램
  - 추가, 조회, 저장 기능

### 8교시: 기초 과정 종합 실습 ⭐⭐⭐
- **복습 퀴즈 (10분)**: Day 1-5 핵심 개념
- **🟢 기초 Problem (15분)**: 클래스 + JSON 저장 시스템
- **🟡 응용 Problem (20분)**: 여러 개념 조합 프로그램 (클래스 + 타입 힌트 + JSON)
- **🔴 도전 Problem (5분)**: 창의적 확장 문제

---

## 📌 핵심 학습 목표 (FastAPI 중심)

### 최우선 항목 ⭐⭐⭐
1. **딕셔너리**: JSON의 기초, API 데이터 구조
2. **타입 힌트**: Pydantic 모델의 핵심
3. **함수 (매개변수, *args, **kwargs)**: 엔드포인트 작성
4. **클래스 (기초)**: Pydantic BaseModel 이해
5. **None과 Optional**: 선택적 필드 처리
6. **데코레이터 개념**: @app.get, @app.post 이해
7. **JSON**: 데이터 직렬화

### 중요 항목 ⭐⭐
1. 리스트
2. 조건문, 반복문
3. 예외 처리
4. 문자열 (f-string)
5. Boolean, Truthy/Falsy
6. import 문법

### 기본 항목 ⭐
1. 튜플
2. 집합
3. while문
4. 람다 함수
5. isinstance()

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
```

### Jupyter vs .py 파일 사용 가이드
- **Day 1-2**: Jupyter 노트북 위주 (즉각적 피드백)
- **Day 3**: 혼용 (딕셔너리는 Jupyter, 제어문은 .py)
- **Day 4-5**: .py 파일 중심 (실무 환경 적응)

### 난이도 표시
- 🟢 기초: 오늘 배운 내용만
- 🟡 응용: 이전 내용 + 오늘 내용
- 🔴 도전: 창의적 사고 필요

### 주의사항

**1. 사전 과제 확인**
- Day 1 시작 전에 환경 구축 완료 확인
- 트러블슈팅 시간을 별도로 확보

**2. f-string 집중**
- % 포매팅, .format()은 "옛날 방식"이라고만 언급 (1분)
- f-string에 충분한 시간 투자

**3. 딕셔너리 중요성 강조**
- FastAPI의 핵심은 JSON = Python 딕셔너리
- 3.5교시 할애는 충분히 가치 있음

**4. 타입 힌트 필수**
- Pydantic 이해를 위해 필수
- 2교시 투자는 응용 과정의 밑거름

**5. None과 Truthy/Falsy**
- Day 1에서 맛보기만
- Day 3-4에서 if문과 함께 제대로
- Day 4-3에서 None 기본값 패턴

**6. JSON은 기초에서**
- 웹 맥락 없이도 딕셔너리 복습용으로 가치 있음
- Day 6에서 웹 맥락 추가 설명

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
- [ ] 간단한 클래스 작성
- [ ] 타입 힌트 추가
- [ ] JSON 파일 저장/로드
- [ ] import로 라이브러리 사용
- [ ] 예외 처리 (try-except)

### 응용 과정 준비 상태:
- [ ] FastAPI 설치 준비 완료
- [ ] JSON 개념 이해
- [ ] 타입 힌트 익숙함
- [ ] 딕셔너리 자유자재
- [ ] 함수 패턴 이해

---

**최종 수정일**: 2026-01-29
**버전**: 3.0
**주요 변경 사항**:
- type() Day 1-2교시에 추가
- Truthy/Falsy Day 3-4교시로 이동
- None 기본값 Day 4-3교시에 추가
- isinstance() Day 5-3교시로 집중
- JSON Day 5-7교시에 추가 (모듈 만들기 제외)
- Day 1-7교시 복습 시간 추가
- 집합 5-7분으로 확대
