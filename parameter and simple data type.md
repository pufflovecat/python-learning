# 变量和简单的数据类型

## 变量

### 变量的命名和使用

* 变量名只能包含字母，数字，下划线
* 变量名不能包含空格
* 不要将python关键字和函数名作变量名
* 变量名应简单且有描述性

### 使用变量时避免命名错误

python编辑器会提供traceback

* 使用变量前忘了赋值
* 输入变量时拼写不正确

## 字符串

python中用引号括起来的就是字符串（单，双）

### 使用方法修改字符串的大小

```python
name = 'ada lovelace'
print(name.title()) 
print(name.upper())
print(name.lower())
```

### 合并字符串

用 + 来合并字符串

```python
firstname = 'yan'
lastname = 'wang'
name = firstname + ' '+lastname
print(name)
```

### 使用制表符或换行符来添加空白

\t  增加空格

\n 用来换行

### 删除空白

因为 "python " （后有空格）和 “python"看起来差不多，但是实际是不一样的，所以要做删除空白的处理

```python
a = 'python '
print(a)
a.rstrip() #删除末尾的空格
print(a) #仍是末尾有空格的
a = a.rstrip() #只有保存之后才是彻底删除了
a.lstrip() #删除开头
a.strip() #删除两边
```

### 使用字符串时避免语法错误

例如单引号里使用单引号

## 数字

### 整数

” + - * 、“

### 浮点数

### 使用函数 str()避免类型错误

```python
age = 23
message = 'Happy '+ str(age)+' rd Birthday'
```

> The Zen of Python, by Tim Peters
>
> Beautiful is better than ugly.
> Explicit is better than implicit.
> Simple is better than complex.
> Complex is better than complicated.
> Flat is better than nested.
> Sparse is better than dense.
> Readability counts.
> Special cases aren't special enough to break the rules.
> Although practicality beats purity.
> Errors should never pass silently.
> Unless explicitly silenced.
> In the face of ambiguity, refuse the temptation to guess.
> There should be one-- and preferably only one --obvious way to do it.
> Although that way may not be obvious at first unless you're Dutch.
> Now is better than never.
> Although never is often better than *right* now.
> If the implementation is hard to explain, it's a bad idea.
> If the implementation is easy to explain, it may be a good idea.
> Namespaces are one honking great idea -- let's do more of those!

