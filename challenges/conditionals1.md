# Conditionals 1

### !challenge

* type: code-snippet
* language: python3.6
* id: bbd9c4ac-32ee-4474-b697-35173143e155
* title: is_old_enough_to_drink

### !question

Write a function called "is_old_enough_to_drink".
Given a number, in this case an age, "is_old_enough_to_drink" returns whether a person of this given age is old enough to legally drink in the United States.
Notes:
* The legal drinking age in the United States is 21.

```
output = is_old_enough_to_drink(22)
print(output) # --> True
```

### !end-question

### !placeholder

```python

def is_old_enough_to_drink(age):
    # your code here
    pass
```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):
    def test1(self):
        #it "should return True if the age is greater than 21"
        self.assertTrue(main.is_old_enough_to_drink(40),"should return True if age is greater than 21")

    def test2(self):
        #it "should return true if the age is 21"
        self.assertTrue(main.is_old_enough_to_drink(21),"should return True if age is 21")

    def test3(self):
        #it "should return false if the age is 20"
        self.assertFalse(main.is_old_enough_to_drink(20),"should return False if age is less than 21")

```

### !end-tests

### !explanation

```python
def is_old_enough_to_drink(age):
    return age >= 21
```
### !end-explanation

### !end-challenge

### !challenge

* type: code-snippet
* language: python3.6
* id: 4b181e05-9f6d-4e2d-beaa-ad80ab8d3c26
* title: is_old_enough_to_drive

### !question

Write a function called "is_old_enough_to_drive".
Given a number, in this case an age, "is_old_enough_to_drive" returns whether a person of this given age is old enough to legally drive in the United States.
Notes:
* The legal driving age in the United States is 16.

```
output = is_old_enough_to_drive(22)
print(output) # --> True
```

### !end-question

### !placeholder

```python
def is_old_enough_to_drive(age):
    # your code here
    pass
```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):
    def test1(self):
        #it "should return true if the age is 16"
        self.assertTrue(main.is_old_enough_to_drive(16),"it should return True if the age greater than or equal to 16")

    def test2(self):
        #it "should return false if the age is less than 16"
        self.assertFalse(main.is_old_enough_to_drive(15),"it should return False if the age is under 16")
```

### !end-tests

### !explanation

```python
def is_old_enough_to_drive(age):
    return age >= 16
```
### !end-explanation

### !end-challenge

### !challenge

* type: code-snippet
* language: python3.6
* id: 8aa5586d-36c6-4677-bd29-bbadd91027b8
* title: is_old_enough_to_vote

### !question

Write a function called "is_old_enough_to_vote".
Given a number, in this case an age, 'is_old_enough_to_vote' returns whether a person of this given age is old enough to legally vote in the United States.
Notes:
* The legal voting age in the United States is 18.

```
output = is_old_enough_to_vote(22)
print(output) # --> True
```

### !end-question

### !placeholder

```python
def is_old_enough_to_vote(age):
    # your code here
    pass
```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):
    def test1(self):
        #it "should return whether the age is greater than 18"
        self.assertTrue(main.is_old_enough_to_vote(19), "should return True if age is greater than 18")

    def test2(self):
        #it "should return true if the age is 18"
        self.assertTrue(main.is_old_enough_to_vote(18), "should return True if age is 18")

    def test3(self):
        #it "should return false if the age is under 18"
        self.assertFalse(main.is_old_enough_to_vote(17), "should return False if age is under 18")     
```


### !end-tests

### !explanation

```python
def is_old_enough_to_vote(age):
    return age >= 18
```
### !end-explanation

### !end-challenge

### !challenge

* type: code-snippet
* language: python3.6
* id: 4031a186-73da-4384-95c9-8d8510aa67a9
* title: is_old_enough_to_drink_and_drive

### !question

Write a function called "is_old_enough_to_drink_and_drive".
Given a number, in this case an age, "is_old_enough_to_drink_and_drive" returns whether a person of this given age is old enough to legally drink and drive in the United States.
Notes:
* The legal drinking age in the United States is 21.
* It is always illegal to drink and drive in the United States.

```
output = is_old_enough_to_drink_and_drive(22)
print(output) # --> False
```

### !end-question

### !placeholder

```python
def is_old_enough_to_drink_and_drive(age):
    # your code here
    pass
```

### !end-placeholder

### !tests

```python
import main
import unittest

class TestScript(unittest.TestCase):
    def test1(self):
        # it "should return false"
        self.assertFalse(main.is_old_enough_to_drink_and_drive(99), "No one is old enough to drink and drive.")
```


### !end-tests

### !explanation
```python
def is_old_enough_to_drink_and_drive(age):
    return False
```
### !end-explanation

### !end-challenge
