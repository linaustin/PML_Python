# Python Data Type Introduction

## 變數(Variable)與資料型態(Data type)

*  數字 (整數、長整數、浮點數)
*  字串 (任意的文字)
*  布林值 (True/False)
*  可變列表(list) (有順序、可變動的資料合集)
*  固定列表(tuple) (有順序、不可變動的資料合集)
*  集合(set) (無順序的資料合集) 
*  字典(dictionary) (鍵值對(key-value pair)的合集)
*  變數(variable) (可用來存放資料的自訂名稱)
<br>

```python

#數字

#整數
3456

#浮點數
3.5

#字串
"測試中文"
"Hello world"

#布林值
True
False

#List(有順序、可變動)
[3, 4, 5]
["Hello", "world"]

#Tuple(有順序、不可變動)
(3, 4, 5)
("Hello", "world")

#Set (無順序)
{3, 4, 5}
{"Hello", "world"}

#Dictionary (key-value pair)
{"apple":"蘋果", "data":"資料", "car":"汽車"}

#變數 用來儲存資料的自訂名稱
#變數名稱 = 資料
x = 3
#print(資料)
print(x)

x = True
print(x)

```
<br>

##  資料基本運算

### 數字運算

```python

#基本加、減
x = 3+6
print(x)  #9

#乘法
x = 3*6
print(x)  #18

#小數除法(答案有小數)
x = 3/6
print(x)  #0.5

#整數除法(答案都是整數)
x = 3//6
print(x)  #0

#次方運算
x = 2**3
print(x)  #8

x = 2**0.5
print(x)  #1.414

#取餘數
x = 7%3
print(x)  #1

#將變數的數字+1
x = 1
x +=1  
print(x)  #2

```
<br>

### 字串運算

```python

#使用雙引號或是單引號都可以建立字串

#跳脫(反斜線)
s = "hell\"o"
print(s)  #hell"o 在字串中使用雙引號

#字串的串接
s = "hello"+"world"
print(s)

#多行文字(使用\n或是三個雙引號)
s = "hello\nworld"
print(s)

s = """hello

world"""
print(s)

#字串的重複
s = "hello"*3 +"world"
print(s)

#字串會對內部字元編號(索引)，從0開始算
s = "hello"  # 0:h  1:e  2:l  3:l  4:o
print(s[0])  #h
print(s[1:4])  #ell
print(s[1:])  #ello
print(s[:4])  #hell

```
<br>

### 有序列表運算(List & Tuple)

```python

#List
grades = [12, 60, 15, 70, 90]
print(grades)
print(grades[0])  #取得特定資料

grades[0] = 55  #修改第一筆資料
print(grades)

#List 子陣列
grades = [12, 60, 15, 70, 90]
print(grades[1:4])

#List 連續刪除資料
grades = [12, 60, 15, 70, 90]
grades[1:4] = []  #連續刪除列表中編號1到編號4(不包含)的資料
print(grades)
print(grades[1])  #90

#List 串接
grades = [12, 60, 15, 70, 90]
grades = grades+[12, 33]
print(grades)

#取得列表的長度
grades = [12, 60, 15, 70, 90]
length = len(grades)
print(length)  #5

#巢狀List
data = [[3, 4, 5], [6, 7, 8]]
print(data[0][1])  #4

data[0][0:2] = [1, 2, 3]
print(data)

#tuple
data = (3, 4, 5)
print(data)
print(data[1])
print(data[0:2])

#data[0] = 5  error:tuple資料不可變動，可以串接



```