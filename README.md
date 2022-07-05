# Python 함수 정리

### Count("문자열")
문자열 데이터에 특정 문자 개수가 몇 개인지 반환하는 함수이다.     
EX)    
```
a = "ASSFSFSF"   
b = a.count("A")    
print(b)    
```
출력값 : 1

### Find("문자열")    
문자열 데이터에 특정 문자의 위치를 반환해주는 함수이다.    
EX)    
```
a = "ASSS_FSFS"
b = a.find("_")
print(b)
```
출력값 : 4 

### upper()

문자열을 모두 대문자로 변경해주는 함수이다.    
EX)
```
a = "asdasFS"
b = a.upper()
print(b)
```
출력값 : ASDASFS

### lower()

문자열을 모두 소문자로 변경해주는 함수이다.    
EX)
```
a = "ASDSDasf"
b = a.lower()
print(b)
```
출력값 : asdsdasf

### append(x)
문자열에 x를 추가하는 함수이다.    
EX)
```
nums = [1,2,3] # list 형식의 data
nums.append(4)
print(nums)
```
출력값 : [1,2,3,4]

```
nums = [1,2,3]
nums.append([5,6])
print(nums)
```
출력값 : [1,2,3,[5,6]]    
append한 [5.6]리스트가 하나의 객체로 추가된다.

### insert(i,x)
문자열에서 원하는 위치(i) 앞에 추가할 값 x를 삽입하는 함수이다.
EX)    
```
nums=[1,2,3]
nums.insert(0, 1) # 0번째(맨앞에) 추가
print(nums)
```
출력값 : [1,1,2,3]

### format 함수
문자열을 출력할 때 변수를 일일이 집어 넣을필요 없이 변수를 받아주는 함수    
'{인덱스0},{인덱스1}'.format(값0, 값1)    
EX) 구구단 만들기    
```
a = 2
b = 3
s ="구구단 {0} x {1} = {2}".format(a,b,a*b)
print(s)
```
출력값 : 구구단 2x3=6

### 리스트 인덱싱

```
a = [1,2,3]
print(a[0])
print(a[1])
print(a[2])
```
결과값 :     
1    
2    
3    

리스트 뿐만 아니라 문자열도 이와 같음

```
a = "ASDASD"
print(a[0])
print(a[1])
print(a[2])
print(a[3])
```
결과값 :     
A    
S    
D    
A    

### 문자열 더하기
문자열을 더해서 출력하는 방법    
EX)    
```
a = "ABC"
b = "abc"
c = a + b
print(c)
```
출력값 : ABCabc

### 리스트 슬라이싱 (중요)
리스트의 원하는 부분만 잘라내서 가져오는 방법, 대괄호와 콜론 : 을 이용해서 진행한다.
EX)    
```
a = [1,2,3,4,5]
print(a[1:4])
```
결과값 : [2,3,4]

이는 문자열에도 동일하게 적용된다.    
EX)    
```
a = "ABCDEF"
print(a[1:4])
```
출력값 : BCD

파이썬 내장 함수가 나열된 wikiDocs    
https://wikidocs.net/32   

파이썬 연산자 종류 정리 Blog
https://dingrr.com/blog/post/python-103-%EC%97%B0%EC%82%B0%EC%9E%90%EC%9D%98-8%EA%B0%80%EC%A7%80-%EC%A2%85%EB%A5%98    

python list에 관련한 함수 (인덱싱, 슬라이싱 등등)    
https://velog.io/@falling_star3/%ED%8C%8C%EC%9D%B4%EC%8D%AC%EC%9D%98-%EB%A6%AC%EC%8A%A4%ED%8A%B8List%EC%99%80-%EA%B4%80%EB%A0%A8-%ED%95%A8%EC%88%98%EB%93%A4append-insert-remove-pop-extend
