def squareEach(num1, num2, num3): #return three values, each squared

    sq1=num1**2
    sq2=num2**2
    sq3=num3**2
    return sq1, sq2, sq3

def sumList(lst): #sums the squared nums from first func
    return sum(lst)

num1,num2,num3=eval(input("Enter three integers: "))
square=squareEach(num1,num2,num3)
sum_of_Squared=sumList(square)
print(sum_of_Squared)

```
class Student(object):
    def __init__(self, name, age, gender, level, grades=None):
        self.name = name
        self.age = age
        self.gender = gender
        self.level = level
        self.grades = grades or {}

    def setGrade(self, course, grade):
        self.grades[course] = grade

    def getGrade(self, course):
        return self.grades[course]

    def getGPA(self):
        return sum(self.grades.values())/len(self.grades)

# Define some students
john = Student("John", 12, "male", 6, {"math":3.3})
jane = Student("Jane", 12, "female", 6, {"math":3.5})

# Now we can get to the grades easily
print(john.getGPA())
print(jane.getGPA())
```

Python is also an Object Oriented Language. You can similarly structure code using OOPs style of coding. But obviously python has a different syntax than javascript in which we have written our code in the past.