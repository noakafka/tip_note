# PYTHON TIP NOTE

# for loop
- basic
for i in range(n) : <------------ 0 부터 n-1 까지

- with list
data = [1, 2, 3]
for item in data : <----------item에 data[0], data[1] ... 이 대입

# list
- pop & remove
list.pop(by idx)
  list.pop(-1) <--------제일 마지막 idx
list.remove(by value)


# dictionary
- 선언
dic = {}

- 접근
value = dic["noa"]   <----- 'noa'의 쌍을 반환 e.g) {'noa':1, 'kafka':2} 이면 1을 반환

- 데이터 변경
dic['noa'] = 3

- 데이터 삭제
del dic['noa']

-존재여부 확인
if 'noa' in dic : <-------true or false


# 순열과 조합
- import
from itertools import permutation

- 순열 Usage
data = [1, 2, 3]
list(map(''.join, permutations(data)))    <----- 1,2,3 / 1,3,2 / 2,1,3 / 2,3,1 / 3,1,2 / 3,2,1
list(map(''.join, permutations(data), 2)) <----- 1,2 / 1,3 / 2,1 / 2,3 / 3,1 / 3,2

- 조합 Usage
data = [1, 2, 3]
num = 3 (or 2...)
list(itertools.combinations(data, num))
