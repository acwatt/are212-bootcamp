Send out the following quiz 2 weeks before the workshop with the following message:
> If you miss one or more question on the quiz, we strongly suggest you attend the workshop

## 1. What do the following lines print?
```python
import numpy as np
X = np.random.rand(100,100)
X1 = X[:, 2]
X2 = X[:, [2]]
print(X1.shape, X2.shape)
```

Options to choose from
```python
(100,1) (100,2)
(100,100) (100,100)
(100,) (100,1)  # correct
(0,) (0,1)
"I don't know"
```

## 2. Given the following code block, which of the options below correctly raises each element of the numpy array X to the 4th power?

```python
import pandas as pd
X = pd.Series([1,2,3,4])
K = 4
def raisePower(x, k):
	return x**k
```

Options to choose from
```python
X.raisePower(x,K)
X.apply(raisePower(K))
X.apply(lambda raisePower(4))
X.apply(lambda x: raisePower(x, K))  # correct
"I don't know"
```

## 3. Consider the following class definition. Which of the options below correctly instantiates a student named Luisa (e.g., which creates a new student object with the name Luisa)?
```python
import numpy as np

class Student:
	def __init__(self, name, grades, age):
		self.name = name
		self.grades = grades
		self.age = age
	
	def greeting(self, phrase):
		print(phrase + ', ' + self.name + '!')
	
	def gpa(self):
		return np.mean(self.grades)
```

Options to choose from
```python
luisa = Student("Luisa", [10,9], 23)  # correct
luisa = Student()
luisa = Student(self, "Luisa", [10,9], 23)
luisa = Student("Luisa")
"I don't know"
```

## 4. Consider the same class definition as before. Assume we have already correctly instantiated the object `luisa`.  Which line correctly returns Luisa's GPA?
```python
import numpy as np

class Student:
	def __init__(self, name, grades, age):
		self.name = name
		self.grades = grades
		self.age = age
	
	def greeting(self, phrase):
		print(phrase + ', ' + self.name + '!')
	
	def gpa(self):
		return np.mean(self.grades)
```

Options to choose from
```python
gpa()
luisa.gpa()  # correct
gpa(luisa)
luisa.gpa(self)
"I don't know"
```

## 5. Consider a modified class definition and method call below. What will this code print?
```python
import numpy as np

class Student:
	def __init__(self):
		self.grades = [4,4,4]
	
	def gpa(self):
		return np.mean(grades)

luisa = Student()
print(luisa.gpa())
```

Options to choose from
```python
# NameError: name 'grades' not defined  # correct
# NameError: name 'np' not defined
# NameError: name 'luisa' not defined
4.0
"I don't know"
```

## 6. Consider again the following class. Which of the following options **only includes methods** of the class?
```python
import numpy as np

class Student:
	def __init__(self, name, grades, age):
		self.name = name
		self.grades = grades
		self.age = age
	
	def greeting(self, phrase):
		print(phrase + ', ' + self.name + '!')
	
	def gpa(self):
		return np.mean(self.grades)
```

Options to choose from
```python
greeting, gpa, self
name, grades, age
self, name, grades, age
__init__, greeting, gpa
"I don't know"
```
