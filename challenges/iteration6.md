# Iteration 6

### !challenge

* type: code-snippet
* language: python3.6
* id: 49c67b68-aa6f-4fc6-a5b9-f1de6a3c8079
* title: multiply_between

### !question

Write a function called "multiply_between".

Given 2 integers, "multiply_between" returns the product between the two given integers, beginning at num1, and excluding num2.

Notes:
* The product between 1 and 4 is 1 * 2 * 3 = 6.
* If num2 is not greater than num1, it should return 0.
```
output = multiply_between(2, 5)
print(output) # --> 24
```

### !end-question

### !placeholder

```python
# your code here



```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):

    def test_0(self):
        # it should return an int
        self.assertIsInstance(main.multiply_between(4, 8), int,
        msg = 'should return an int')


    def test_1(self):
        # it should multiply between the first and second number exclusive
        self.assertEqual(main.multiply_between(4, 6), 20,
        msg = 'should multiply between the first and second number, exclusive')


    def test_2(self):
        # it should multiply between the first and second number when they are one number apart
        self.assertEqual(main.multiply_between(4, 5), 4,
        msg = 'should multiply between the first and second number when they are one number apart')


    def test_3(self):
        # it should multiply between the first and second number exclusive with negatives
        self.assertEqual(main.multiply_between(-5, -3), 20,
        msg = 'should multiply between the first and second number exclusive with negatives')


    def test_4(self):
        # it should return 0 if the second number is less than the first
        self.assertEqual(main.multiply_between(1, -3), 0,
        msg = 'should return 0 if the second number is less than the first')


    def test_5(self):
        # it should return 0 if the 2 numbers are equal
        self.assertEqual(main.multiply_between(1, 1), 0,
        msg = 'should return 0 if the 2 numbers are equal')


```
### !end-tests

### !explanation
```python
def multiply_between(num1, num2):
    if num2 <= num1: return 0
    acc = 1
    for i in range(num1, num2):
        acc *= i
    return acc

#alternative solution
# from functools import reduce
# def multiply_between(num1, num2):
#     try:
#         return reduce(lambda x,y: x*y, range(num1, num2))
#     except:
#         return 0
```
### !end-explanation

### !end-challenge

### !challenge

* type: code-snippet
* language: python3.6
* id: fc489cfd-7046-4452-8557-c1fccc5ba5a5
* title: sum_between

### !question

Write a function called "sum_between".

Given 2 integers, "sum_between" returns the sum between the two given integers, beginning at num1, and excluding num2.

Notes:
* The sum between 1 and 4 is 1 + 2 + 3 = 6.
* If num2 is not greater than num1, it should return 0.
```
output = sum_between(2, 5)
print(output) # --> 9
```

### !end-question

### !placeholder

```python
# your code here



```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):
    def test_0(self):
        # it should return an int
        self.assertIsInstance(main.sum_between(4, 8), int,
        msg = 'should return an int')


    def test_1(self):
        # it should sum between the first and second number exclusive
        self.assertEqual(main.sum_between(4, 6), 9,
        msg = 'should sum between the first and second number, exclusive')


    def test_2(self):
        # it should sum between the first and second number exclusive with negatives
        self.assertEqual(main.sum_between(-1, 3), 2,
        msg = 'should sum between the first and second number exclusive with negatives')


    def test_3(self):
        # it should return 0 if the second number is less than the first
        self.assertEqual(main.sum_between(1, -3), 0,
        msg = 'should return 0 if the second number is less than the first')


    def test_4(self):
        # it should return 0 if the 2 numbers are equal
        self.assertEqual(main.sum_between(1, 1), 0,
        msg = 'should return 0 if the 2 numbers are equal')

```

### !end-tests

### !explanation
```python
from functools import reduce
def sum_between(num1, num2):
    try:
        return reduce(lambda x, y: x + y, range(num1, num2))
    except:
        return 0
```
### !end-explanation

### !end-challenge
