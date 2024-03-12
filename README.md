## Python
- **Python Syntax**
1. **Python Indentation**

⚠️  **들여쓰기를 건너뛰면 오류가 발생, 일반적으로는 4개가 사용되지만 적어도 1개는 있어야 한다**

```언어
if 5 > 2;
print("Five is greater than Two!")
```

```언어
if 5 > 2;
	print("Five is greater than Two!")
```

2. **Python Variables** 

   **변수에 값을 할당하면 변수가 생성된다**

```언어
x = 5
y = "Hello World!"
```

3. **Comment** 

   **#을 통해 주석을 달 수 있다**

```언어
#이것은 주석입니다
print("Hello World")
```

- **Python Comments**
1. **주석은 #으로 시작되고 그 뒤는 Python에서 무시된다**

```언어
#이것은 주석입니다
print("Hello World")
```

2. **삼중 따옴표를 사용해 그 안에 주석을 넣을 수 있다**

```언어
"""
이것은 주석입니다
이것은 주석입니다
이것은 주석입니다
"""
print("Hello World")
```

- **Python Variables**
1. **변수는 처음 할당하는 순간 생성된다**

```언어
x = 5
y = "Saaly"
print(x)
print(y)
```

2. **변수는 특정 유형으로 설정할 필요가 없고 설정된 후에 유형을 변경할 수 있다**

```언어
x = 5       # int는 정수형으로 작성된 변수
x = "Sally" # str은 문자열로 작성된 변수
print(x)

```

3. **다양한 유형으로 변수를 설정할 수 있다**

```언어
x = int(3)
y = str(3)
z = float(3) # float은 실수형으로 작성된 변수
```

4. **함수를 사용하면 변수의 데이터 유형을 알 수 있다**

```언어
x = 5
y = "Sally"
print(type(x))
print(type(y))
```

5. **문자열 변수는 ‘나 “를 사용하여 선언할 수 있다**

```언어
x = 'sally'
x = "Sally"
# 둘은 똑같다
```

6. **변수 이름은 대소문자를 구별한다**

```언어
a = 5
A = "Sally
# 둘은 같지 않다
```

- **Python Variables - Variable Names**
1. **변수 이름은 문자나 밑줄 문자로 시작해야 한다**
2. **변수 이름은 숫자로 시작할 수 없다**
3. **변수 이름에는 영문,숫자와 밑줄(Az, 0-9 및 _)만 포함할 수 있다**
4. **변수 이름은 대소문자를 구분한다. (age, Age 및 AGE는 세 가지 다른 변수이다)**

```언어
myvar = "Sally"
my_var = "Sally"
_my_var = "Sally"
myVar = "Sally"
MYVAR = "Sally"
myvar2 = "Sally"
```

- **Python Variables - Assign Multiple Values**
1. **한 줄로 여러 변수에 값을 할당할 수 있다**

```언어
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```

2. **한 줄에 여러 변수에 동일한 값을 할당할 수 있다**

```언어
x = y = z = "orange"
print(x)
print(y)
print(z)
```

3. **값들이 모여있는 컬렉션이 있는 경우 Python을 사용하면 값을 변수로 추출할 수 있다**

```언어
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
```

- **Python Variables - Output Variables**
1. **‘print’함수는 변수를 출력하는데 많이 사용된다**

```언어
x = "Python is awesome"
print(x)
```

2. **‘print’함수에서는 여러 변수를 쉼표로 구분하여 출력한다**

```언어
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
```

3. **+를 사용해서 여러 변수를 출력할 수 있다**

```언어
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)
```

4. **숫자의 경우, +는 수학 연산자로 사용된다**

```언어
x = 5
y = 10
print(x + y)
```

5.  **‘print’함수에서 문자열과 숫자를 +와 결합하려고 하면 오류가 발생한다**

```언어
x = 5
y = "Sally"
print(x + y)
```

6. **함수에서 여러 변수를 출력하는 가장 좋은 방법은 ‘print’변수를 쉼표로 구분하는 것이다**

```언어
x = 5
y = "Sally"
print(x, y)
```

- **Python Variables - Global Variables**
1. **전역 변수는 함수 내부와 외부 모두에서 사용할 수 있다**

```언어
x = "awesome"

def myfunc():
  print("Python is " + x)

myfunc()
```

2. **전역 변수와 동일한 이름을 사용하여 함수 내부에 변수를 만든다**

```언어
x = "awesome"

def myfunc():
  x = "fantastic"
  print("Python is " + x)

myfunc()

print("Python is " + x)
```

3. **키워드를 사용하면 ‘global’변수는 전역 범위에 속한다**

```언어
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

4. **’global’함수 내에서 전역 변수를 변경하려면 키워드를 사용해야 한다**

```언어
x = "awesome"

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

- **Python Data Types**

| 텍스트 유형 | str |
| --- | --- |
| 숫자 유형 | int, float, complex |
| 시퀀스 유형 | list, tuple, range |
| 매핑 유형 | dict |
| 세트 유형 | set,frozenset |
| 부울 유형 | bool |
| 바이너리 유형 | bytes, bytearray, memoryview |
| 없음 유형 | NoneType |
1. **함수를 사용하면 변수의 데이터 유형을 알 수 있다**

```언어
x = 5
y = "Sally"
print(type(x))
print(type(y))
```

- **Python Numbers**
1. **Python에는 세 가지 숫자 유형이 있다**

   **`int` , `float` , `complex`**

2. **숫자 유형의 변수는 값을 할당하면 생성된다**

```언어
x = 1    # int
y = 2.8  # float
z = 1j   # complex
```

2. **한 유형에서 다른 유형으로 변환할 수 있다**

```언어
x = 1    # int
y = 2.8  # float
z = 1j   # complex

#float으로 바꾸기:
x = float(1)

#int로 바꾸기:
y = int(2.8)

#complex로 바꾸기:
z = complex(1)

print(x)
print(y)
print(z)

print(type(x))
print(type(y))
print(type(z))

```

- **Python Strings**
1. **‘안녕하세요’와 “안녕하세요”는 같다**

```언어
print("Hello")
print('Hello')
```

2. **변수에 문자열을 할당하는 것은 변수 이름 뒤에 등호와 문자열이 오는 방식으로 수행된다**

```언어
a = "고마워"
print(a)
```

3. **세 개의 따옴표를 사용하여 여러 줄 문자열을 변수에 할당할 수 있다**

```언어
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)
```

- **Python Strings - Slicing Strings**
1. **슬라이스 구문을 사용하여 다양한 문자를 반환할 수 있다**

```언어
b = "Hello, World!"
print(b[2:5])
```

2. **시작 인덱스를 생략하면 범위는 첫 번째 문자에서 시작된다**

```언어
b = "Hello, World!"
print(b[:5])
```

3. **끝 인덱스를 생략하면 범위가 끝으로 이동한다**

```언어
b = "Hello, World!"
print(b[2:])
```

4. **문자열 끝에서 조각을 시작하려면 음수 인덱스를 사용한다**

```언어
b = "Hello, World!"
print(b[-5:-2])
```

- **Python Strings - Modify Strings**
1. **upper함수는 문자열을 대문자로 반환한다**

```언어
a = "Hello, World!"
print(a.upper())
```

2. **lower함수는 문자열을 소문자로 반환한다**

```언어
a = "Hello, World!"
print(a.lower())
```

3. **strip함수는 시작이나 끝에서 공백을 제거한다**

```언어
a = " Hello, World! "
print(a.strip())
```

4. **replace함수는 문자열을 다른 문자열로 바꾼다**

```언어
a = "Hello, World!"
print(a.replace("H", "J"))
```

5. **split함수는 구분 기호의 인스턴스를 찾으면 문자열을 하위 문자열로 분할한다**

```언어
a = "Hello, World!"
b = a.split(",")
print(b)
```

- **Python Strings - String Concatenation**
1. **a변수 와 b변수를 c변수로 병합하기**

```언어
a = "Hello"
b = "World"
c = a + b
print(c)
```

2. **사이에 공백을 추가하려면  ” “을 추가해야 한다**

```언어
a = "Hello"
b = "World"
c = a + " " + b
print(c)
```

- **Python Strings - Format**
1. **format함수를 사용하면 문자열과 숫자를 결합할 수 있다**

```언어
age = 36
txt = "My name is John, and I am {}"
print(txt.format(age))
```

2. **인덱스 번호를 사용하여 `{0}`인수가 올바른 자리에 배치되었는지 확인할 수 있다**

```언어
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price)) 
```

- **Python Strings  - Escape Characters**
1. **이스케이프 문자를 사용하면 일반적으로 허용되지 않는 큰따옴표를 사용할 수 있다**

```언어
txt = "We are the so-called \"Vikings\" from the north."
print(txt) 
```

- **Python Booleans**

  **부울은  `True`또는 `False` 두 값 중에 하나를 나타낸다**

1. **if 문에서 조건을 실행하면 Python은 `True`또는`False` 를 반환한다**

```언어
print(10 > 9)
print(10 == 9)
print(10 < 9)
```

2. **bool함수를 사용하면 모든 값을 평가하고**  `
   **True또는 False를 제공한다**

```언어
print(bool("Hello"))
print(bool(15))
```

3. **True를 반환한다**

```언어
print(bool("abc"))
print(bool(123))
print(bool(["apple", "cherry", "banana"]))
```

4. **False를 반환한다**

```언어
print(bool(False))
print(bool(None))
print(bool(0))
print(bool(""))
print(bool(()))
print(bool([]))
print(bool({}))
```

- **Python Lists**
1. **목록은 대괄호를 사용하여 생성된다**

```언어
thislist = ["apple", "banana", "cherry"]
print(thislist)
```

2. **목록에서는 중복 값을 허용한다**

```언어
thislist = ["apple", "banana", "cherry", "apple", "cherry"]

print(thislist)
```

3. **목록에 포함된 항목 수를 확인하려면 다음 `len()`함수를 사용해야 한다**

```언어
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
```

4. **Python의 관점에서 목록은 'list' 데이터 유형을 가진 객체로 정의된다**

```언어
<class 'list'>
```

5. **새 목록을 만들 때 list() 생성자를 사용하는 것도 가능하다**

```언어
thislist = list(("apple", "banana", "cherry"))
print(thislist)

```

- **Python Tuples**

  **튜플은 순서가 지정되고 변경할 수 없는 컬렉션이다**

1. **튜플은 둥근 괄호로 작성된다**

```언어
thistuple = ("apple", "banana", "cherry")
print(thistuple)
```

2. **튜플은 중복 값을 허용한다**

```언어
thistuple = ("apple", "banana", "cherry", "apple", "cherry")
print(thistuple)
```

- **Python Sets**

  **세트는 단일 변수에 여러 항목을 저장하는 데 사용됩니다.**

  **세트는 순서가 없고, 변경할 수 없으며, 색인이 생성되지 않은 컬렉션이다**

1. **세트는 중괄호로 작성된다**

```언어
thisset = {"apple", "banana", "cherry"}
print(thisset)
```

2. **set() 생성자를 사용하여 세트를 만든다**

```언어
thisset = set(("apple", "banana", "cherry"))
print(thisset)
```

- **Python Dictionaries**

  **사전은 키:값 쌍으로 데이터 값을 저장하는 데 사용된다**

  **사전은 순서가 지정되고 변경 가능하며 중복이 허용되지 않는 모음이다**

1. **사전은 중괄호로 작성되며 키와 값을 갖는다**

```언어
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)
```

- **Python If ... Else**
1. **"if 문"은 if 키워드를 사용하여 작성된다**

```언어
a = 33
b = 200

if b > a:
  print("b is greater than a")
```

2. **elif 키워드 는 "이전 조건이 true가 아니면 이 조건을 시도하십시오"라고 말하는 방식이다**

```언어
a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
```

3. **else 키워드 는 이전 조건에서 포착되지 않은 모든 항목을 포착한다**

```언어
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
```

4. **and 키워드 는 논리 연산자이며 조건문을 결합하는 데 사용된다**

```언어
a = 200
b = 33
c = 500
if a > b and c > a:
  print("Both conditions are True")
```
6. **키워드 `or`는 논리 연산자이며 조건문을 결합하는 데 사용된다**

```언어
a = 200
b = 33
c = 500
if a > b or a > c:
  print("At least one of the conditions is True")
```

7. **키워드 `not`는 논리 연산자이며 조건문의 결과를 뒤집는 데 사용된다**

```언어
a = 33
b = 200
if not a > b:
  print("a is NOT greater than b")
```

- **Python While Loop**
1. **while 루프를 사용하면 조건이 참인 한 일련의 명령문을 실행할 수 있다**

```언어
i = 1
while i < 6:
  print(i)
  i += 1
```

  **while 루프를 사용하려면 관련 변수가 준비되어 있어야 한다**

  **이 예에서는 인덱싱 변수 i 를 정의하고 이를 1로 설정해야 한다**

2. **break 문을 사용하면 while 조건이 true인 경우에도 루프를 중지할 수 있다**

```언어
i = 1
while i < 6:
  print(i)
  if (i == 3):
    break
  i += 1
```

3.  **continue 문을 사용하면 현재 반복을 중지하고 다음을 계속할 수 있다**

```언어
i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
```

4. **else 문을 사용하면 조건이 더 이상 참이 아닐 때 코드 블록을 한 번 실행할 수 있다**

```언어
i = 1
while i < 6:
  print(i)
  i += 1
else:
  print("i is no longer less than 6")
```

- **Python For Loop**

**for 루프는 시퀀스(즉, 목록, 튜플, 사전, 집합 또는 문자열)를 반복하는 데 사용된다**

**for 루프를 사용하면 목록, 집합 등의 각 항목에 대해 한 번씩 일련의 명령문을 실행할 수 있다**

```언어
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x) 
```

1. **문자열도 반복 가능한 객체이므로 일련의 문자를 포함한다**

```언어
for x in "banana":
  print(x) 
```

2. **break 문을 사용하면 모든 항목을 반복하기 전에 루프를 중지할 수 있다**

```언어
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x) 
  if x == "banana":
    break
```

3. **continue 문을 사용하면 루프의 현재 반복을 중지하고 다음을 계속할 수 있다**

```언어
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    continue
  print(x) 
```

4. **지정된 횟수만큼 코드 세트를 반복하려면 range() 함수를 사용할 수 있다**

```언어
for x in range(6):
  print(x) 
```

5. **else`루프 의 키워드는 루프 `for`가 완료될 때 실행될 코드 블록을 지정한다**

```언어
for x in range(6):
  print(x)
else:
  print("Finally finished!")
```
