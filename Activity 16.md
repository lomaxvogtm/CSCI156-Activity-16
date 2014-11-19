### Class Employee
1. Create a class Employee
```python
class Employee:
    pass
```
### Input SS#
2. Create a procedure that has an argument of type Employee and inputs their SS# into Employee.ss (substitute you instance variable for Employee here). Your code should validate that a valid SS# is put in.
3. Create an exception InvalidSocial. In the event that an invalid ss# is typed in raise this exception.
4. Your code can be pilfered from the previous activity, with some modification. The outline is below, where all you need to do is fill in validate

```python
class InvalidSocial(ValueError):
    pass

class Employee:
    pass

def validatess(employee_class):
    check that employee_class.ss is valid
    Anywhere that you find the ss is invalid raise InvalidSocial
    
def getsocial(employee_class):
    employee_class.ss = input("Social: ")
    try
        validatess(employee_class)
    except InvalidSocial:
        print("Invalid SS, please try again\n")
        getsocial(employee_class)

emp = Employee()
getsocial(emp)
print(emp.ss)
```
