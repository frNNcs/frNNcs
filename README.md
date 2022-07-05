<h3>

```python
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple = ("Python", "JS", "PHP")
    databases   : tuple = ("PostgreSQL", "MYSQL", "MSSQL", "Redis")
    misc        : tuple = ("Docker", "Celery", "RabbitMQ", "CI/CD")
    ongoing     : tuple = ("Django", "DRF", "nodejs", "solidity")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
```
</h3>
