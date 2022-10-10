# homework
## 1 *https://edabit.com/challenge/gt9LLufDCMHKMioh2*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')

def stutter(word):
	return word[0:2] + '... ' + word[0:2] + '... ' + word + '?'

actual_param, expected_param = [
	"increasing", "adventures", "enticing", "unacceptable", "accountable", "incredible", "exquisite",
	"am", "enduring", "outstanding", "astonishing", "astounding", "impressive", "revolutionize",
	"recurring", "recollection", "so", "gorgeous", "captivating"
], [
	"in... in... increasing?", "ad... ad... adventures?", "en... en... enticing?", "un... un... unacceptable?",
    "ac... ac... accountable?", "in... in... incredible?", "ex... ex... exquisite?", "am... am... am?",
    "en... en... enduring?", "ou... ou... outstanding?", "as... as... astonishing?", "as... as... astounding?",
    "im... im... impressive?", "re... re... revolutionize?", "re... re... recurring?", "re... re... recollection?",
    "so... so... so?", "go... go... gorgeous?", "ca... ca... captivating?",
]
for i, w in enumerate(actual_param):
	Test.assert_equals(stutter(w), expected_param[i])
______________________________________________________________________
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
```

## 2 *https://edabit.com/challenge/cXnkmRdxqJrwdsP4n*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')
def dis(price, discount):
  return round(price - (price*(discount/100)),2)

Test.assert_equals(dis(100, 75), 25)
Test.assert_equals(dis(211, 50), 105.5)
Test.assert_equals(dis(593, 61), 231.27)
Test.assert_equals(dis(1693, 80), 338.6)
Test.assert_equals(dis(700, 10), 630)
_________________________________________________________
Passed
Passed
Passed
Passed
Passed
```
## 3 *https://edabit.com/challenge/2X2uZysLJ3CpsxLDD*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')
import math
def radians_to_degrees(rad):
  return round(rad*180/math.pi, 1)

Test.assert_equals(radians_to_degrees(1), 57.3)
Test.assert_equals(radians_to_degrees(5), 286.5)
Test.assert_equals(radians_to_degrees(7), 401.1)
Test.assert_equals(radians_to_degrees(60), 3437.7)
Test.assert_equals(radians_to_degrees(100), 5729.6)
Test.assert_equals(radians_to_degrees(180), 10313.2)
_____________________________________________
Passed
Passed
Passed
Passed
Passed
Passed
```

## 4 *https://edabit.com/challenge/4me7LifXBwj5rhL4n*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')
import math
def circle_or_square(rad, area):
  s1=2*math.pi*rad
  s2=4*(area**0.5) 
  if s1>s2: a=True 
  else: a=False
  return a

Test.assert_equals(circle_or_square(16, 625), True)
Test.assert_equals(circle_or_square(8, 144), True)
Test.assert_equals(circle_or_square(15, 400), True)
Test.assert_equals(circle_or_square(5, 100), False)
Test.assert_equals(circle_or_square(18, 900), False)
Test.assert_equals(circle_or_square(1, 4), False)
__________________________________
Passed
Passed
Passed
Passed
Passed
Passed 
```

## 5 *https://edabit.com/challenge/HYjQKDXFfeppcWmLX*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')
import math
def is_curzon(num):
  if (2**num+1) % (2*num+1)==0: return True
  else: return False

Test.assert_equals(is_curzon(5), True)
Test.assert_equals(is_curzon(10), False)
Test.assert_equals(is_curzon(14), True)
Test.assert_equals(is_curzon(86), True)
Test.assert_equals(is_curzon(90), True)
Test.assert_equals(is_curzon(115), False)
Test.assert_equals(is_curzon(120), False)
Test.assert_equals(is_curzon(194), True)
Test.assert_equals(is_curzon(293), True)
_____________________________________
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
```

## 6 *https://edabit.com/challenge/3DAkZHv2LZjgqWbvW*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')

def is_adjacent(matrix, n1, n2):
  return matrix[n1][n2]

matrix = [[0,1,0,0],[1,0,1,1],[0,1,0,1],[0,1,1,0]]
Test.assert_equals(is_adjacent(matrix, 0, 1), True)
Test.assert_equals(is_adjacent(matrix, 0, 2), False)
Test.assert_equals(is_adjacent(matrix, 2, 1), True)

matrix = [[0,1,0,1,1], [1,0,1,0,0],[0,1,0,1,0],[1,0,1,0,1],[1,0,0,1,0]]
Test.assert_equals(is_adjacent(matrix, 0, 3), True)
Test.assert_equals(is_adjacent(matrix, 1, 4), False)
Test.assert_equals(is_adjacent(matrix, 3, 2), True)
____________________________________________________
Passed
Passed
Passed
Passed
Passed
Passed
```
## 7 *https://edabit.com/challenge/xRMQG4Sxewx5agDRr*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')

def find_highest(lst):
  m =0
  for i in lst:
    if i>m: m=i
  return m

Test.assert_equals(find_highest([8]), 8)
Test.assert_equals(find_highest([-1, 3, 5, 6, 99, 12, 2]), 99)
Test.assert_equals(find_highest([0, 12, 4, 87]), 87)
___________________________________________________
Passed
Passed
Passed
```
## 8 *https://edabit.com/challenge/zkKNmC66ASvSm5wJA*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')

def perimeter(l, num):
  return (l == 's')*4*num + (l == 'c')*6.28*num

Test.assert_equals(perimeter("s", 1), 4)
Test.assert_equals(perimeter("s", 4), 16)
Test.assert_equals(perimeter("s", 9), 36)
Test.assert_equals(perimeter("s", 13), 52)
Test.assert_equals(perimeter("s", 30), 120)
Test.assert_equals(perimeter("c", 1), 6.28)
Test.assert_equals(perimeter("c", 4), 25.12)
Test.assert_equals(perimeter("c", 9), 56.52)
Test.assert_equals(perimeter("c", 13), 81.64)
Test.assert_equals(perimeter("c", 30), 188.4)
______________________________________________
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
Passed
```
## 9 *https://edabit.com/challenge/MtktG9Dz7z9vBCFYM*
```py
class Test:
    def assert_equals(a, b, *args, **kwargs):
        assert a == b
        print('Passed')

import socket
def get_domain(ip_address): 
  return socket.gethostbyaddr(ip_address)[0]

Test.assert_equals(get_domain("8.8.8.8"), "dns.google")
Test.assert_equals(get_domain("8.8.4.4"), "dns.google")
_______________________________________________________
Passed
Passed

```
