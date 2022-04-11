---
title:  "[파이썬] 기초 연산"
date:   2020-12-20 15:04:23
categories: [Python]
tags: [Python]
---

파이썬에 관한 첫 포스트..는 역시 신텍스부터라고 생각한다. 내 1차학기 강좌중 파이썬으로 딥러닝을 실습하는 강좌가 있기도하고, high level이라 배우기도 쉽고 가벼우니 공부해보기로 했다!  
파이썬은 들여쓰기(indentation)
  
참고서적: [점프투파이썬]으로 교수님 추천이다.


##1. 연산자  
**연산**하는건 아주 쉽다.
1. 사칙연산은 (+,-,*,/) 그대로 계산한다.  
2. `**` 은 제곱값을 Return한다.
3. `%` 은 나머지를 Return한다.
4. `//`은 몫을 Return한다.

```python
>>> a = 3
>>> b = 4
>>> a ** b 
81  
'''
% 활용
'''
>>> 7 % 3 
1
'''
// 와 / 의 차이점
'''
>>> 7 / 4
1.75
>>> 7 // 4 
1

```
  
___

##2. 문자열 연산  
**문자열**: String 으로 글자, 단어 등 다 String으로 표현할 수 있다.  
또한 수(int, float)가 아니기 때문에 큰따옴표("")나 작은따옴표('')를 넣어 문자열 표기한다.

[점프투파이썬] 2장에 따르면, 문자열 안에 따옴표를 포함시키려면 아래와 같이 한다.

|case|description|example|
|:---:|:---:|---|
' '| 문자열 안에 넣을 시엔 큰따옴표로 묶기 | ex) "Python's favorite" |   
" "| 문자열 안에 넣을 시엔 작은따옴표로 묶기 | ex) '"Python is very easy." he says.'|

또한 자바와 같게 백슬래시를 사용하기도 한다.

```python
>>> say = "\"Python is very easy.\" he says."
>>> food = 'Python\'s favorite food is perl
```  

여러 줄인 문자열은 \n을 삽입하거나 따옴표 3개를 사용한다.
|case|example|
|:---:|---|
|\n| `multiline = "Life is too short\nYou need python"`|
|""".'''| >>> multiline=''' </br>Life is too short </br>You need python </br>'''|

### 문자열 더하기/곱하기
```python
'''
더하기 예시
'''
>>> head = "Python"
>>> tail = "is fun!"
>>> head + tail
'Python is fun!'

'''
곱하기 예시
'''
>>> a = "python"
>>> a * 2
'pythonpython'

'''
곱하기 응용: multistring.py 의 header을 설정하면 제목보기가 편하다!
'''
# multistring.py
print("="*50)
print("My Program")
print("="*50)
```






[점프투파이썬]: https://wikidocs.net/book/1