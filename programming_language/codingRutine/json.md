# jackson

## json_encode/json_decode

### php

```php
$obj = StdClass();
$obj.name = "ada";
$obj.age = 17;

echo json_encode($obj);
```

### python

```python
import json

class Human:
    def __init__(self, name, age):
        self.name = name
        self.age = age


man = Human('ada', 17)
s = json.dumps(man.__dict__)
print(s)
```

### java

```java
import com.fasterxml.jackson.databind.ObjectMapper;
import lombok.Data;

// ...
@Data
class Human {
    String name;
    Integer age;
}

// ...
Human man = new Human();
man.setName("Lion");
man.setAge(19);

ObjectMapper mapper = new ObjectMapper();
String json = null;
try {
    json = mapper.writeValueAsString(man);
} catch (JsonProcessingException e) {
    e.printStackTrace();
}
System.out.println(json);
```