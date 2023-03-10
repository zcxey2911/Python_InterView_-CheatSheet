
#解释一下Python中的三元运算

```
[on true] if [expression] else [on false]
```
如果表达式为True，就执行[on true]中的语句。否则，就执行[on false]中的语句

```
a,b=2,3
min=a if a<b else b
min
```


##GIL: 全局解释器锁（英语：Global Interpreter Lock，缩写GIL），是计算机程序设计语言解释器用于同步线程的一种机制，它使得任何时刻仅有一个线程在执行。[1]即便在多核心处理器上，使用 GIL 的解释器也只允许同一时间执行一个线程。



#解释一下Python中的继承

当一个类继承自另一个类，它就被称为一个子类/派生类，继承自父类/基类/超类。它会继承/获取所有类成员（属性和方法）。

继承能让我们重新使用代码，也能更容易的创建和维护应用。Python支持如下种类的继承：

单继承：一个类继承自单个基类
多继承：一个类继承自多个基类
多级继承：一个类继承自单个基类，后者则继承自另一个基类
分层继承：多个类继承自单个基类
混合继承：两种或多种类型继承的混合



#解释Python中的help()和dir()函数

Help()函数是一个内置函数，用于查看函数或模块用途的详细说明：

```
import copy
help(copy.copy)
```

Dir()函数也是Python内置函数，dir() 函数不带参数时，返回当前范围内的变量、方法和定义的类型列表；带参数时，返回参数的属性、方法列表。

```
dir(copy.copy)
```

#什么是猴子补丁？

在运行期间动态修改一个类或模块。

```
class A:
    def func(self):
        print("Hi")
def monkey(self):
    print("Hi, monkey")
m.A.func = monkey
a = m.A()
a.func()
```

#请解释使用*args和**kwargs的含义

当我们不知道向函数传递多少参数时，比如我们向传递一个列表或元组，我们就使用*args。

```
>>> def func(*args):
    for i in args:
        print(i)  
>>> func(3,2,1,4,7)
```

在我们不知道该传递多少关键字参数时，使用**kwargs来收集关键字参数。

```
>>> def func(**kwargs):
    for i in kwargs:
        print(i,kwargs[i])
>>> func(a=1,b=2,c=7)
```

#什么是负索引？

负索引和正索引不同，它是从右边开始检索。

它也能用于列表中的切片：

```
mylist=[0,1,2,3,4,5,6,7,8]
mylist[-3]
mylist[-6:-1]
```

#解释Python中的join()和split()函数

Join()能让我们将指定字符添加至字符串中。

Split()能让我们用指定字符分割字符串。

#怎么移除一个字符串中的前导空格？

字符串中的前导空格就是出现在字符串中第一个非空格字符前的空格。我们使用方法Istrip()可以将它从字符串中移除。

```
'   Ayushi '.lstrip()
```
可以看到，该字符串既有前导字符，也有后缀字符，调用Istrip()去除了前导空格。如果我们想去除后缀空格，就用rstrip()方法。
```
'   Ayushi '.rstrip()
```

#Python中的pass语句是什么？

在用Python写代码时，有时可能还没想好函数怎么写，只写了函数声明，但为了保证语法正确，必须输入一些东西，在这种情况下，我们会使用pass语句。

```
def func(*args):
    pass 
```

同样，break语句能让我们跳出循环。

```
for i in range(7):
    if i==3: break
```

最后，continue语句能让我们跳到下个循环。
```
for i in range(7):
    if i==3: continue
    print(i)
```


#Python中的闭包是什么？

当一个嵌套函数在其外部区域引用了一个值时，该嵌套函数就是一个闭包。其意义就是会记录这个值。

```
def A(x):
    def B():
        print(x)
    return B
```

#谈一谈Python的装饰器（decorator）

装饰器本质上是一个Python函数，它可以让其它函数在不作任何变动的情况下增加额外功能，装饰器的返回值也是一个函数对象。它经常用于有切面需求的场景。比如：插入日志、性能测试、事务处理、缓存、权限校验等。有了装饰器我们就可以抽离出大量的与函数功能无关的雷同代码进行重用。

装饰器其实就是一个闭包，把一个函数当做参数然后返回一个替代版函数



#解释一下Python中的逻辑运算符

Python中有3个逻辑运算符：and，or，not

#Python支持什么数据类型？
1. Numbers（数字）——用于保存数值

2. Strings（字符串）——字符串是一个字符序列。我们用单引号或双引号来声明字符串。

3. Lists（列表）——列表就是一些值的有序集合，我们用方括号声明列表。

4. Tuples（元组）——元组和列表一样，也是一些值的有序集合，区别是元组是不可变的，意味着我们无法改变元组内的值。

5. Dictionary（字典）——字典是一种数据结构，含有键值对。我们用大括号声明字典

#什么是切片？

切片是Python中的一种方法，能让我们只检索列表、元素或字符串的一部分。在切片时，我们使用切片操作符[]。

```
(1,2,3,4,5)[2:4]
```

#Python中的不可变集合（frozenset）是什么？

首先，我们讨论一下什么是集合。集合就是一系列数据项的合集，不存在任何副本。另外，集合是无序的。

这就意味着我们无法索引它。

不过，集合是可变的。而不可变集合却不可变，这意味着我们无法改变它的值，从而也使其无法作为字典的键值。

```
myset=frozenset([1,3,2,2])
myset
```

#解释lambda表达式，什么时候会用到它？

如果我们需要一个只有单一表达式的函数，我们可以匿名定义它。拉姆达表达式通常是在需要一个函数，但是又不想费神去命名一个函数的场合下使用，也就是指匿名函数。

```
(lambda a,b:a if a>b else b)(3,3.5)
```

实现斐波那契数列
```
fib = lambda n : n if n <= 2 else fib(n-1)+fib(n-2)
```


#什么是递归？

在调用一个函数的过程中，直接或间接地调用了函数本身这个就叫递归。但为了避免出现死循环，必须要有一个结束条件

```
def facto(n):
    if n==1: return 1
    return n*facto(n-1)
facto(4)
```

#什么是生成器？

生成器会生成一系列的值用于迭代，这样看它又是一种可迭代对象。它是在for循环的过程中不断计算出下一个元素，并在适当的条件结束for循环。

#什么是迭代器？

迭代器是访问集合元素的一种方式。迭代器对象从集合的第一个元素开始访问，直到所有的元素被访问完结束。迭代器只能往前不会后退。我们使用inter()函数创建迭代器。

#请说说生成器和迭代器之间的区别?

在使用生成器时，我们创建一个函数；在使用迭代器时，我们使用内置函数iter()和next()。
在生成器中，我们使用关键字‘yield’来每次生成/返回一个对象。
生成器中有多少‘yield’语句，你可以自定义。
每次‘yield’暂停循环时，生成器会保存本地变量的状态。而迭代器并不会使用局部变量，它只需要一个可迭代对象进行迭代。
使用类可以实现你自己的迭代器，但无法实现生成器。
生成器运行速度快，语法简洁，更简单。
迭代器更能节约内存。

#Python中的yield用法

yield简单说来就是一个生成器，这样函数它记住上次返 回时在函数体中的位置。对生成器第 二次(或n 次)调用跳转至该函 次)调用跳转至该函数。

#解释Python的参数传递机制

Python使用按引用传递（pass-by-reference）将参数传递到函数中。如果你改变一个函数内的参数，会影响到函数的调用。这是Python的默认操作。不过，如果我们传递字面参数，比如字符串、数字或元组，它们是按值传递，这是因为它们是不可变的。

python不允许程序员选择采用传值还是传引用。Python参数传递采用的肯定是“传对象引用”的方式。这种方式相当于传值和传引用的一种综合。如果函数收到的是一个可变对象（比如字典或者列表）的引用，就能修改对象的原始值－－相当于通过“传引用”来传递对象。如果函数收到的是一个不可变对象（比如数字、字符或者元组）的引用，就不能直接修改原始对象－－相当于通过“传值'来传递对象。

#如何在Python中创建自己的包？

Python中创建包是比较方便的，只需要在当前目录建立一个文件夹，文件夹中包含一个__init__.py文件和若干个模块文件，其中__init__.py可以是一个空文件，但还是建议将包中所有需要导出的变量放到__all__中，这样可以确保包的接口清晰明了，易于使用。

#元类

元类是类的类对象，换言之类是元类的实例，Python中默认的元类为type，可以通过自定义元类的方式实现对类创建的控制。

```
class Base:
    a = 1
    b = 2

    print('class defined')

    def __new__(cls, *args, **kwargs):
        print(cls.__name__, 'class instance created')
        return super().__new__(cls)

    def __init__(self):
        print(type(self).__name__, 'class instance inited')

    def hello(self):
        pass


b = Base()
```

当调用print(type(b))，得到<class ‘main.Base’>，可知b是Base类的实例。Python是纯面向对象语言，因此类也是对象，当调用print(type(Base))时得到<class ‘type’>，可知类Base是type的实例，type就是Python中的原生元类，用来控制、生成类这个对象。
一般地，在定义类时，默认的此类的元类是type，因此，如果我们想控制类的创建，需要将类的元类指为我们自定义的元类，这个自定义的元类需要继承type元类。


