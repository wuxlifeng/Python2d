# [ThinkPython-en-cn](https://github.com/wuxlifeng/ThinkPython-en-cn) 读书笔记





[12.4](https://github.com/wuxlifeng/ThinkPython-en-cn/blob/master/ThinkPython-12.md#124--variable-length-argument-tuples-参数长度可变的元组) Variable-length argument tuples

Many of the built-in functions use variable-length argument tuples. For example, max and min can take any number of arguments:

```python
>>> max(1, 2, 3)
3
```
But sum does not.

As an exercise, write a function called sumall that takes any number of arguments and returns their sum.

```python
# TRY
def sumall(*t): 
    return sum(t) 
# run and surprise, 
>>> sumall(1, 2,3)
>>> 6 ## OK
>>> t = range(1, 101)
>>> sumall(*t)  # * is needed.
>>> sumall(*range(1, 100)
````

Note:
* `python` after `'''` is needed, then keep it 完整：`'''python`
* documentation functoion [sum](https://docs.python.org/3/library/functions.html?highlight=sum#sum) 
  * math.fsum()
  * itertools.chain()
    * yield

[12.6](https://github.com/wuxlifeng/ThinkPython-en-cn/blob/master/ThinkPython-12.md#126--dictionaries-and-tuples-词典与元组)
* ??

[13.7 前联系 6](https://github.com/wuxlifeng/ThinkPython-en-cn/blob/master/ThinkPython-13.md#exercise-6-练习6)
* 2016-10-12 19:10:58
