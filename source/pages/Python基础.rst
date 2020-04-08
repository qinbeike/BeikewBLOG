python基础
#####################

前言
*********************

python是一种动态强类型的解释型语言，动态是指运行期间确定类型，相对的，静态是在编译时确定类型。强类型是指在没有强制类型转化前，不允许两种不同类型的变量互相操作，”一旦一个变量被指定了某个数据类型，如果不经过强制转换，那么它就永远是这个数据类型了“。例如::

    a = 1
    b = '1'
    c = a + b
    输出如下：
    Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
    TypeError: unsupported operand type(s) for +: 'int' and 'str'

第一章 python数据类型
***********************

python的六大数据类型：数字类型、字符串、字典、元组、列表、集合

1.1 数字类型
==============

数字类型包括int、float、complex、bool

python中常用的进制包括b:二进制、o:八进制、d:十进制、x:十六进制；可以使用bin()、oct()、hex()将十进制转为相应进制的字符串；

其它进制转十进制：int('123',8) ;"{:d}".format((0x123));eval('0x123')

十进制转其它进制：bin(123)、oct(123)、hex(123);"{:b}".format(123)、"{:o}".format(123)、"{:x}".format(123)

其它常用函数::

    round(x,n):返回浮点数x的四舍五入值，小数点保留n位，需要注意的是python中4.5是4.4999999，round时结果为4
    divmod(x,y):返回商和余数的元组
    power(x,n):返回x的n次方



1.2 字符串
=============

python中没有字符类型，只有字符串，可以用单引号、双引号
字符串常用方法：
len()
str()
s.lower()
char.join(sequence):将要连接的元素序列用字符char连接起来，常用的有''.join(sequence)
str.strip():用于移除字符串头尾指定的字符，默认为空格
ord(c):返回字符串的ASCII值，c为字符串

1.3 字典
================

字典是由键和值组成的

字典的常用方法：
dictname.setdefault(key, defaultvalue):key不存在时设置的默认键值
dict.keys(): 以列表形式返回字典的所有键
dict.items():返回可迭代的(key,value)的元组



第一章 常用内置函数及语法糖
***********************

lambda x,y:x+y (1,1)