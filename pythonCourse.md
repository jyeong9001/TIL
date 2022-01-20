# Returns

함수의 주 사용 목적으로는 값을 돌려받는 것이다. 함수에서 값을 돌려받기 위해서는 함수안에 return이 있어야 한다.

```python
def p_plus(a,b);
  print(a+b)

def r_plus(a,b);
  return a+b

p_result = p_plus(2,3)
r_result = r_plus(2,3)

# 변수 선언 & 초기화문이 있다면 우변 => 좌변의 방향으로 진행

print (p_result, r_result)

# 5
# None 5

# (1) p_plus라는 함수를 2와 3이라는 전달인자 (Arguments)와 함께 실행
# (2) p_plus 함수 내부의 print(a + b)가 실행, 이때 a는 2, b는 3. 따라서 5가 출력됨
# (3) p_plus는 출력만 하지 리턴하는 결과가 없음
# - None이 아닌 어떤 값을 반환(리턴)하면 리턴값이 있지만, 아무것도 리턴하지 않으면 None이 리턴됨
# (4) p_plus(2, 3)의 결과로 반환된 None이 p_result에 저장됨
```

주의할 점은 함수내에서 return이 실행되는 순간 그 뒤에 얼마나 많은 실행문이 있던지간에 해당 function은 바로 종료된다는 사실이다.

```python
def r_plus(a,b);
  return a+b
  print("lalalala")

r_result = r_plus(2, 4)

print(r_result)

#6
```

# Keyworded arguments

- positional argument: position에 따른 방식
- keyword argument: value를 부여하는 방식

string 안에 변수명을 써주고 싶을 때, 변수이름에는 중괄호를 써주고 string 맨 앞에 f를 붙여준다.

```python
f"hello {name} you are {age} years old"
```

이 때, argument의 순서를 신경쓰고 싶지 않을 때
hello = say_hello (age="12", name="nico") 로 표기 가능하다. argument가 많아지면, 순서를 실수할 수 있기 때문에 이 방법도 중요하다

# Web scrapper

beautifulsoup은 html에서 정보를 추출하기에 유용한 package이다.
먼저 package에서 requests와 beautifulsoup4를 install 받는다.
