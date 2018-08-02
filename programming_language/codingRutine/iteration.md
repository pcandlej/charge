# Iteration

## for/foreach

### php

```php
<?php
$arr = ["name": "ada", "age": 17];
foreach ($arr as $k => $v) {
    echo $k . ":" . $v;
}
```

### python

```python
dict = {'name': 'ada', 'age': 17}
for k, v in dict.items() :
    print(str(k) + ":" + str(v))
```

### java

```java
Map<String, String> myDict = new HashMap<>();
myDict.put("name", "ada");
myDict.put("age", 17);

myDict.forEach((k, v) -> System.out.println(String.format("%s : %s", k, v)));
```
