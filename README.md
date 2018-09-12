# python-DI-lambda-factory
This Dependency Injection, lambda and factory in python example shows how to create a python class that gets a formatter injected to keep the class free of print statements.

```
vera = Employee("Vera", 35000)
chuck = Employee("Chuck", 29000)

formatter = lambda employee : print(f"{employee.name} earns {employee.salary}")

report = EmployeeReport(formatter)
report.print([vera, chuck])
```

output:

```
Vera earns 35000
Chuck earns 29000
```
