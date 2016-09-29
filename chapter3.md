
## 练习三

换行如此：`print('+ \n -')`，而非例三提示：`print('+', '-') `

接行如此可以：
```python
print('+', end=' ')
print('-') 
```



如下的代码根据样例二改变而来：

```python
from __future__ import print_function, division


def do_twice(func, arg):
    """Runs a function twice.

    func: function object
    arg: argument passed to the function
    """
    func(arg)
    func(arg)


def print_twice(arg):
    """Prints the argument twice.

    arg: anything printable
    """
    print(arg)
    print(arg)


def do_four(func, arg):
    """Runs a function four times.

    func: function object
    arg: argument passed to the function
    """
    do_twice(func, arg)
    do_twice(func, arg)


print               ('+----------------+----------------+-----------------+')
do_four(print_twice, '|                |                |                 |')
print               ('+----------------+----------------+-----------------+')
do_four(print_twice, '|                |                |                 |')
print               ('+----------------+----------------+-----------------+')
do_four(print_twice, '|                |                |                 |')
print               ('+----------------+----------------+-----------------+')
```
输出结果如下：

```
+----------------+----------------+-----------------+
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
+----------------+----------------+-----------------+
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
+----------------+----------------+-----------------+
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
|                |                |                 |
+----------------+----------------+-----------------+
```
疑问：
* 打印换行, [参见第四章](https://github.com/wuxlifeng/ThinkPython-en-cn/blob/master/ThinkPython-04.md#42--simple-repetition-简单的重复)
```python
for i in range(4):     
    print('Hello!') 
```
