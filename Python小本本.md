# 函数

##### 1.1定义一个函数：

```
def fn():
	print('这是我的第一个函数！')
	
fn()
```

fn是函数对象 fn() 调用函数

print是函数对象 print() 调用函数

```
##函数简介( function )
-函数也是个对象
-对象是内存中专门用来存储数据的一块区域
-函数可以用来保存一些可执行的代码，并且可以在需要时，对这些语句进行多次的调用-创建函数︰
def函数名([形参1,形参2,...形参n]) :
代码块
-函数名必须要符号标识符的规范
(可以包含字母、数字、下划线、但是不能以数字开头)
-函数中保存的代码不会立即执行，需要调用函数代码才会执行-调用函数:
函数对象()
-定义函数─般都是要实现某种功能的
##函数的参数
-在定义函数时，可以在函数名后的()中定义数量不等的形参，
多个形参之间使用,隔开
-形参（形式参数），定义形参就相当于在函数内部声明了变量，但是并不赋值
-实参(实际参数)
如果函数定义时,指定了形参,那么在调用函数时也必须传递实参，
实参将会赋值给对应的形参，简单来说,有几个形参就得传几个实参

```





# 字符元组等基础

```
1、字符本体转换
lower() 返回小写的字符串：
a = "Hello, World!"
print(a.lower())

upper() 方法返回大写的字符串：
a = "Hello, World!"
print(a.upper())

replace() 用另一段字符串来替换字符串：
a = "Hello, World!"
print(a.replace("World", "Kitty"))

split() 方法在找到分隔符的实例时将字符串拆分为子字符串：
a = "Hello, World!"
print(a.split(","))
# returns ['Hello', ' World!']

您可以使用索引号 {0} 来确保参数被放在正确的占位符中：
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price))
I want to pay 49.95 dollars for 3 pieces of item 567.

capitalize()   把首字符转换为大写。
casefold() 把字符串转换为小写。
center()   返回居中的字符串。
count()    返回指定值在字符串中出现的次数。
encode()   返回字符串的编码版本。
endswith() 如果字符串以指定值结尾，则返回 true。
expandtabs()   设置字符串的 tab 尺寸。
find() 在字符串中搜索指定的值并返回它被找到的位置。
format()   格式化字符串中的指定值。
format_map()   格式化字符串中的指定值。
index()    在字符串中搜索指定的值并返回它被找到的位置。
isalnum()  如果字符串中的所有字符都是字母数字，则返回 True。
isalpha()  如果字符串中的所有字符都在字母表中，则返回 True。
isdecimal()    如果字符串中的所有字符都是小数，则返回 True。
isdigit()  如果字符串中的所有字符都是数字，则返回 True。
isidentifier() 如果字符串是标识符，则返回 True。
islower()  如果字符串中的所有字符都是小写，则返回 True。
isnumeric()    如果字符串中的所有字符都是数，则返回 True。
isprintable()  如果字符串中的所有字符都是可打印的，则返回 True。
isspace()  如果字符串中的所有字符都是空白字符，则返回 True。
istitle()  如果字符串遵循标题规则，则返回 True。
isupper()  如果字符串中的所有字符都是大写，则返回 True。
join() 把可迭代对象的元素连接到字符串的末尾。
ljust()    返回字符串的左对齐版本。
lower()    把字符串转换为小写。
lstrip()   返回字符串的左修剪版本。
maketrans()    返回在转换中使用的转换表。
partition()    返回元组，其中的字符串被分为三部分。
replace()  返回字符串，其中指定的值被替换为指定的值。
rfind()    在字符串中搜索指定的值，并返回它被找到的最后位置。
rindex()   在字符串中搜索指定的值，并返回它被找到的最后位置。
rjust()    返回字符串的右对齐版本。
rpartition()   返回元组，其中字符串分为三部分。
rsplit()   在指定的分隔符处拆分字符串，并返回列表。
rstrip()   返回字符串的右边修剪版本。
split()    在指定的分隔符处拆分字符串，并返回列表。
splitlines()   在换行符处拆分字符串并返回列表。
startswith()   如果以指定值开头的字符串，则返回 true。
strip()    返回字符串的剪裁版本。
swapcase() 切换大小写，小写成为大写，反之亦然。
title()    把每个单词的首字符转换为大写。
translate()    返回被转换的字符串。
upper()    把字符串转换为大写。
zfill()    在字符串的开头填充指定数量的 0 值。

```

# Python 集合（数组）

Python 编程语言中有四种集合数据类型：
列表（List）是一种有序和可更改的集合。允许重复的成员。
元组（Tuple）是一种有序且不可更改的集合。允许重复的成员。
集合（Set）是一个无序和无索引的集合。没有重复的成员。
词典（Dictionary）是一个无序，可变和有索引的集合。没有重复的成员。

```
要在指定的索引处添加项目，请使用 insert() 方法：
插入项目作为第二个位置：
thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")
print(thislist)

删除项目
有几种方法可以从列表中删除项目：
remove() 方法删除指定的项目：
thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)

pop() 方法删除指定的索引（如果未指定索引，则删除最后一项）：
thislist = ["apple", "banana", "cherry"]
thislist.pop()
print(thislist)

del 关键字删除指定的索引：（不加索引的话可以完整的删除列表）
thislist = ["apple", "banana", "cherry"]
del thislist[0]
print(thislist)

clear() 方法清空列表：
thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist)

使用 copy() 方法来复制列表：
thislist = ["apple", "banana", "cherry"]
mylist = thislist.copy()
print(mylist)

使用 extend() 方法将 list2 添加到 list1 的末尾：
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]
list1.extend(list2)
print(list1)
```

数组参数汇总：

```
append()	在列表的末尾添加一个元素
clear()	删除列表中的所有元素
copy()	返回列表的副本
count()	返回具有指定值的元素数量。
extend()	将列表元素（或任何可迭代的元素）添加到当前列表的末尾
index()	返回具有指定值的第一个元素的索引
insert()	在指定位置添加元素
pop()	删除指定位置的元素
remove()	删除具有指定值的项目
reverse()	颠倒列表的顺序
sort()	对列表进行排序
```

元组

```
打印元组的最后一个项目：
thistuple = ("apple", "banana", "cherry")
print(thistuple[-1])

使用 tuple() 方法来创建元组：
thistuple = tuple(("apple", "banana", "cherry")) # 请注意双括号
print(thistuple)
```

元组参数汇总：

```
count()	返回元组中指定值出现的次数。
index()	在元组中搜索指定的值并返回它被找到的位置。
```

集合

```
创建集合：
thisset = {"apple", "banana", "cherry"}
print(thisset)

使用 set() 构造函数来创建集合：
thisset = set(("apple", "banana", "cherry")) # 请留意这个双括号
print(thisset)
```

集合参数汇总：

```
add()	向集合添加元素。
clear()	删除集合中的所有元素。
copy()	返回集合的副本。
difference()	返回包含两个或更多集合之间差异的集合。
difference_update()	删除此集合中也包含在另一个指定集合中的项目。
discard()	删除指定项目。
intersection()	返回为两个其他集合的交集的集合。
intersection_update()	删除此集合中不存在于其他指定集合中的项目。
isdisjoint()	返回两个集合是否有交集。
issubset()	返回另一个集合是否包含此集合。
issuperset()	返回此集合是否包含另一个集合。
pop()	从集合中删除一个元素。
remove()	删除指定元素。
symmetric_difference()	返回具有两组集合的对称差集的集合。
symmetric_difference_update()	插入此集合和另一个集合的对称差集。
union()	返回包含集合并集的集合。
update()	用此集合和其他集合的并集来更新集合。
```

字典

```
创建并打印字典：
thisdict =	{
  "brand": "Porsche",
  "model": "911",
  "year": 1963
}
print(thisdict)

获取 "model" 键的值：
x = thisdict["model"]

把 "year" 改为 2019：
thisdict =	{
  "brand": "Porsche",
  "model": "911",
  "year": 1963
}
thisdict["year"] = 2019

使用 values() 函数返回字典的值：
for x in thisdict.values():
  print(x)
  
逐个打印字典中的所有值：
for x in thisdict:
  print(thisdict[x])
  
  
通过使用 items() 函数遍历键和值：
for x, y in thisdict.items():
  print(x, y)
  
将项目添加到字典中：
thisdict =	{
  "brand": "Porsche",
  "model": "911",
  "year": 1963
}
thisdict["color"] = "red"
print(thisdict)

pop() 方法删除具有指定键名的项：
thisdict =	{
  "brand": "Porsche",
  "model": "911",
  "year": 1963
}
thisdict.pop("model")
print(thisdict)

clear() 关键字清空字典：
thisdict =	{
  "brand": "Porsche",
  "model": "911",
  "year": 1963
}
thisdict.clear()
print(thisdict)
```

字典参数汇总：

```
clear()	删除字典中的所有元素
copy()	返回字典的副本
fromkeys()	返回拥有指定键和值的字典
get()	返回指定键的值
items()	返回包含每个键值对的元组的列表
keys()	返回包含字典键的列表
pop()	删除拥有指定键的元素
popitem()	删除最后插入的键值对
setdefault()	返回指定键的值。如果该键不存在，则插入具有指定值的键。
update()	使用指定的键值对字典进行更新
values()	返回字典中所有值的列表
```

类属性

```
使用名为 x 的属性，创建一个名为 MyClass 的类：
class MyClass:
  x = 5
  
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age
p1 = Person("Bill", 63)
print(p1.name)
print(p1.age)

插入一个打印问候语的函数，并在 p1 对象上执行它：
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age
  def myfunc(self):
    print("Hello my name is " + self.name)
p1 = Person("Bill", 63)
p1.myfunc()

class Person:
  def __init__(self, fname, lname):
    self.firstname = fname
    self.lastname = lname
  def printname(self):
    print(self.firstname, self.lastname)
#Use the Person class to create an object, and then execute the printname method:
x = Person("Bill", "Gates")
x.printname()


class Person:
  def __init__(self, fname, lname):
    self.firstname = fname
    self.lastname = lname
  def printname(self):
    print(self.firstname, self.lastname)
class Student(Person):
  def __init__(self, fname, lname):
    Person.__init__(self, fname, lname)
x = Student("Elon", "Musk")
x.printname()

class MyNumbers:
  def __iter__(self):
    self.a = 1
    return self
  def __next__(self):
    if self.a <= 20:
      x = self.a
      self.a += 1
      return x
    else:
      raise StopIteration
myclass = MyNumbers()
myiter = iter(myclass)
for x in myiter:
  print(x)
```

时间date属性

```
%a	Weekday，短版本	Wed
%A	Weekday，完整版本	Wednesday
%w	Weekday，数字 0-6，0 为周日	3
%d	日，数字 01-31	31
%b	月名称，短版本	Dec
%B	月名称，完整版本	December
%m	月，数字01-12	12
%y	年，短版本，无世纪	18
%Y	年，完整版本	2018
%H	小时，00-23	17
%I	小时，00-12	05
%p	AM/PM	PM
%M	分，00-59	41
%S	秒，00-59	08
%f	微妙，000000-999999	548513
%z	UTC 偏移	+0100
%Z	时区	CST
%j	天数，001-366	365
%U	周数，每周的第一天是周日，00-53	52
%W	周数，每周的第一天是周一，00-53	52
%c	日期和时间的本地版本	Mon Dec 31 17:41:00 2018
%x	日期的本地版本	12/31/18
%X	时间的本地版本	17:41:00
%%	A % character	%
```

re正则

```
检索字符串以查看它是否以 "China" 开头并以 "country" 结尾：
import re
txt = "China is a great country"
x = re.search("^China.*country$", txt)
```

re函数：

```
findall	返回包含所有匹配项的列表
search	如果字符串中的任意位置存在匹配，则返回 Match 对象
split	返回在每次匹配时拆分字符串的列表
sub	用字符串替换一个或多个匹配项
```

元字符

```
[]	一组字符	"[a-m]"
\	示意特殊序列（也可用于转义特殊字符）	"\d"
.	任何字符（换行符除外）	"he..o"
^	起始于	"^hello"
$	结束于	"world$"
*	零次或多次出现	"aix*"
+	一次或多次出现	"aix+"
{}	确切地指定的出现次数	"al{2}"
|	两者任一	"falls|stays"
()	捕获和分组
```

特殊序列

```
\A	如果指定的字符位于字符串的开头，则返回匹配项	"\AThe"
\b	返回指定字符位于单词的开头或末尾的匹配项	r"\bain"  r"ain\b"
\B	返回指定字符存在的匹配项，但不在单词的开头（或结尾处）	r"\Bain"  r"ain\B"
\d	返回字符串包含数字的匹配项（数字 0-9）	"\d"
\D	返回字符串不包含数字的匹配项	"\D"
\s	返回字符串包含空白字符的匹配项	"\s"
\S	返回字符串不包含空白字符的匹配项	"\S"
\w	返回一个匹配项，其中字符串包含任何单词字符（从 a 到 Z 的字符，从 0 到 9 的数字和下划线 _ 字符）	"\w"
\W	返回一个匹配项，其中字符串不包含任何单词字符	"\W"
\Z	如果指定的字符位于字符串的末尾，则返回匹配项	"Spain\Z"
```

sub替换函数

```
用数字 9 替换每个空白字符：
import re
str = "China is a great country"
x = re.sub("\s", "9", str)
print(x)

替换前两次出现：
str = "China is a great country"
x = re.sub("\s", "9", str, 2)
print(x)
```

Try Except

```
try 块允许您测试代码块以查找错误。
except 块允许您处理错误。
finally 块允许您执行代码，无论 try 和 except 块的结果如何。
```

```
这对于关闭对象并清理资源非常有用：
试图打开并写入不可写的文件：
try:
  f = open("demofile.txt")
  f.write("Lorum Ipsum")
except:
  print("Something went wrong when writing to the file")
finally:
  f.close()
```

raise关键字用于引发异常

```
如果 x 不是整数，则引发 TypeError：
x = "hello"
if not type(x) is int:
  raise TypeError("Only integers are allowed")
```

命令行输入

```
Python 3.6 中的方法与 Python 2.7 略有不同
Python 3.6 使用 input() 方法
Python 2.7 使用 raw_input() 方法


```

字符串格式化

```
price = 52
txt = "The price is {:.2f} dollars"
print(txt.format(price))
```

文件打开写入创建

```
open（）函数
r  读取 不存在返回错误
a  追加到文件末尾 不存在则创建文件
w  写入覆盖原内容 不存在则创建文件
x  创建指定文件，若存在则返回错误
t  文本模式
b  二进制模式 例如图像
```

文件读取

```
f = open("demofile.txt", "r")
print(f.read(5)) #前五个字符

readline（） 返回一行
print(f.readline())

读取前两行
readline调用两次，例：
print(f.readline())
print(f.readline())

遍历文件的行：
f = open("demofile.txt", "r")
for x in f:
  print(x)
  
最后关闭文件,在某些情况下，由于缓冲，应该始终关闭文件，在关闭文件之前，对文件所做的更改可能不会显示。
f.close()
```

文件删除

```
import os
#删除文件
os.remove('demofile.txt')
#删除文件夹,只能删除空文件
os.rmdir('myfolder')


检查文件是否存在
import os
if os.path.exists("demofile.txt"):
  os.remove("demofile.txt")
else:
  print("The file does not exist")
```

机器学习

```
直方图数据分布
import numpy
import matplotlib.pyplot as plt
#x轴的范围 最大取值
x = numpy.random.uniform(0.0, 5.0, 100000)
#x轴个数展示
plt.hist(x, 100)
#效果展示
plt.show()
```

