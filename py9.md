字符串中的前导空格就是出现在字符串中第一个非空格字符前的空格。我们使用方法Istrip()可以将它从字符串中移除。

```
'   Ayushi '.lstrip()
```
可以看到，该字符串既有前导字符，也有后缀字符，调用Istrip()去除了前导空格。如果我们想去除后缀空格，就用rstrip()方法。
```
'   Ayushi '.rstrip()
```