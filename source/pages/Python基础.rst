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

数字类型
=========

数字类型包括int、float、complex、bool