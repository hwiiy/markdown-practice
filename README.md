# 클래스  
: 붕어빵과 붕어빵 틀에 비유   
이때 `붕어빵 틀`에 해당되는 것이 `'클래스'`  
이 틀을 통해 만들어진 `붕어빵`을 `'객체'`
```python
class Waffle :
  pass

  choco = Waffle()
  banana = Waffle()
```
choco는 객체이다. (O)  
choco는 Waffle의 인스턴스이다. (X)  
<br> </br>

### 객체와 인스턴스
- 객체 : 여러가지 속성을 가질 수 있는 대상  
- 인스턴스 : 클래스를 기반으로 만들어진 객체

### 클래스 활용

```python 
class Calc :
  def setdata(Self,first,second): #setdata 메소드
    self.first = first
    self.second = second
  def add(self): #add 메소드
    result = self.first + self.second
    return result

a = calc()
a.setdata (6,3)
print(a.add()) #9출력
```

### 생성자
: setdata함수보다 안전한 초깃값 설정 가능

```python 
class calc:
  def __init__(self,first,second):
    self.first = first
    self.second = second
  def add(self):
    result = self.first + self.second
    return result

a = calc(6,3) #객체 생성시 초깃값 설정!!
print(a.add()) # 9 출력
```