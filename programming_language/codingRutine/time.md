# Time

## strtotime

### php

* php 的 strtotime 方法返回的数字单位为 秒

```php
<?php
echo strtotime("2018-10-11 12:00:00");
```

### java

* java 返回时间戳时返回的数字单位为 微秒

```java
import org.joda.time.DateTime;

...

DateTime dt = new DateTime("2018-10-11T12:00:00.000+08:00");
System.out.println(dt.toDate().getTime());
```

```java
import org.apache.commons.lang3.time.DateUtils;

...

try {
    System.err.println(DateUtils.parseDate("2018-11-11", "yyyy-MM-dd"));
} catch (ParseException e) {
    e.printStackTrace();
}
```


## date string

### php

```php
<?php
echo date('c', time());
// 2018-08-02T11:03:34+08:00
```


### java

```java
import org.assertj.core.util.DateUtil;
import org.apache.commons.lang.time.DateFormatUtils;

...

Date now = DateUtil.now();
System.err.println(DateFormatUtils.ISO_DATETIME_TIME_ZONE_FORMAT.format(now));
// 2018-08-02T11:27:11+08:00
```
