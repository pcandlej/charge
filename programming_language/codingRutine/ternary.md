# Ternary

## x ? x : y

### php

```php
<?php
$x = 100;
$x = $x == 100 ? $x : 50;
echo $x;

$mydict = ["name" => "Ada", "age" => 17];
echo $mydict["enemy"] ? : "Som"; // Notice: Undefined index
```

### python

```python
x = 100
x = x if x == 100 else 50
print(x)

mydict = {"name":"Ada", "age":17}
print(mydict.get("enemy", "Som"))
```

### java

```java
int x = 100;
x = x == 100 ? x : 50;
System.out.println(x);

Map<String, String> mydict = new HashMap<>();
mydict.put("name", "Ada");
mydict.put("age", "17");
System.out.println(mydict.getOrDefault("enemy", "Som"));
```

