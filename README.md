### Hi there ~ <img src="https://user-images.githubusercontent.com/1303154/88677602-1635ba80-d120-11ea-84d8-d263ba5fc3c0.gif" width="24px" alt="hi">

<h3>
    
```python
​
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple = ("Python", "JS", "PHP")
    databases   : tuple = ("PostgreSQL", "MYSQL", "MSSQL", "Redis")
    misc        : tuple = ("Docker", "Celery", "RabbitMQ", "CI/CD")
    ongoing     : tuple = ("Django", "DRF", "nodejs")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
​
```
</h3>
