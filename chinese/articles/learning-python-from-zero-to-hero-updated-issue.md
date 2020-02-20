> * 原文地址：[Learning Python: From Zero to Hero](https://www.freecodecamp.org/news/learning-python-from-zero-to-hero-120ea540b567/)
> * 原文作者：TK
> * 译者：MMMAY521
> * 校对者：

![Learning Python: From Zero to Hero](https://cdn-media-1.freecodecamp.org/images/1*ueWmI48uuShON-hX7LwI0w.png)
Python学习：从小白到大神(https://cdn-media-1.freecodecamp.org/images/1*ueWmI48uuShON-hX7LwI0w.png)
by TK
作者：TK
First of all, what is Python? According to its creator, Guido van Rossum, Python is a:
第一个问题：Python是什么？Python创始人吉多*范苏罗姆认为，Python是一种
> “high-level programming language, and its core design philosophy is all about code readability and a syntax which allows programmers to express concepts in a few lines of code.”
>“高级编程语言，其核心设计哲学强调代码的可读性和句法，这使得开发人员能够仅仅用几行代码就表达想法。”
For me, the first reason to learn Python was that it is, in fact, a beautiful  programming language. It was really natural to code in it and express my thoughts.
为什么我要学Python呢？一个原因在于，Python是一个美丽的编程语言，用Python编程来表达我的想法非常自然流畅。
Another reason was that we can use coding in Python in multiple ways: data science, web development, and machine learning all shine here. Quora, Pinterest and Spotify all use Python for their backend web development. So let’s learn a bit about it.
另一个原因就是，Python编程在很多方面都大有可为，例如数据科学、网站开发、机器学习等等。Quora， Pinterest和Spotify的后端网站开发都在使用Python。因此，让我们一同来学习Python吧。
### The Basics基础知识

#### 1\. Variables变量

You can think about variables as words that store a value. Simple as that.你可以把变量理解成储存值的代码，很简单。

In Python, it is really easy to define a variable and set a value to it. Imagine you want to store number 1 in a variable called “one.” Let’s do it:在Python中，定义一个变量、给变量赋值十分简单。例如：给变量“one”赋值1，代码如下：

```py
one = 1
```

How simple was that? You just assigned the value 1 to the variable “one.”这样就可以把1赋值给变量“one”了，很简单吧。

```py
two = 2
some_number = 10000
```

And you can assign any other  **value**  to whatever other  **variables** you want. As you see in the table above, the variable “**two**” stores the integer  **2**, and “**some\_number**” stores  **10,000**.你可以把任意数值赋值给你想要的任意变量。如上述代码，变量“**two**”存储了整数2，变量“**some\_number**”存储了整数10000。

Besides integers, we can also use booleans (True / False), strings, float, and so many other data types.除了整数，布尔值（True / False）、字符串、浮点数和其他数据类型也可以赋值给变量。

```py
# booleans
true_boolean = True
false_boolean = False

# string
my_name = "Leandro Tk"

```

#### 2\. Control Flow: conditional statements控制语句：条件判断

“**If**” uses an expression to evaluate whether a statement is True or False. If it is True, it executes what is inside the “if” statement. For example:“**If**”条件语句检验条件真假。如果条件为真，if后面的条件执行。举个例子：

```py
if True:
  print("Hello Python If")

```

**2**  is greater than  **1**, so the “**print**” code is executed.**2**比**1**大，所以**print**后面的程序执行。

The “**else**” statement will be executed if the “**if**” expression is  **false**.如果if后面的条件语句为假，则执行else后面的语句

```py
if 1 > 2:
  print("1 is greater than 2")
else:
  print("1 is not greater than 2")
```

**1**  is not greater than  **2**, so the code inside the “**else**” statement will be executed.1小于2，所以执行else后面的语句。

You can also use an “**elif**” statement:也可以使用elif语句：

```py
if 1 > 2:
  print("1 is greater than 2")
elif 2 > 1:
  print("1 is not greater than 2")
else:
  print("1 is equal to 2")
```

#### 3\. Looping / Iterator循环/迭代

In Python, we can iterate in different forms. I’ll talk about two:  **while** and  **for**.Python有很多不同的迭代模式。今天说两个：while循环和for循环。

**While** Looping: while the statement is True, the code inside the block will be executed. So, this code will print the number from  **1**  to  **10**.while循环：当条件为真，执行while模块语句。所以，while循环可以y用来输出s数字1-10。

```py
num = 1

```

The  **while**  loop needs a “**loop condition.**” If it stays True, it continues iterating. In this example, when  `num`  is  `11`  the  **loop condition**  equals  `False`.while循环需要循环条件。如果循环条件为真，循环继续。上述代码表明，num值为11时，循环条件为假。

Another basic bit of code to better understand it:另外一种代码形式可以更好的理解循环条件：

```py
loop_condition = True

```

The  **loop condition**  is  `True`  so it keeps iterating — until we set it to  `False`.循环条件为真，循环继续，知道循环条件为假。

**For Looping**: you apply the variable “**num**” to the block, and the “**for**” statement will iterate it for you. This code will print the same as  **while**  code: from  **1**  to  **10**.for循环：模块语句运用num变量时，for循环迭代变量。for循环代码可以跟while循环一样输出数字1-10。

```py
for i in range(1, 11):
  print(i)
```

See? It is so simple. The range starts with  `1`  and goes until the  `11`th element (`10`  is the  `10`th element).看见了吧，就是这么简单。整数数列range()循环从1开始，直到第十一个元素停止循环（但只输出第十个元素10）。

### List: Collection | Array | Data Structure列表（List）：集合（Collection）|数组（Array）|数据结构（Data Structure）

Imagine you want to store the integer 1 in a variable. But maybe now you want to store 2. And 3, 4, 5 …设想一下你需要把整数1储存在一个变量中。但现在可能你想储存2，甚至储存3,4,5……

Do I have another way to store all the integers that I want, but not in  **millions of variables**? You guessed it — there is indeed another way to store them.是否有一种方式可以避免将我所想要的所有的整数存在不计其数的变量当中？你已经猜到了——确实有另一种方式来储存这些整数。

`List`  is a collection that can be used to store a list of values (like these integers that you want). So let’s use it:列表（List）这种集合就可以用来储存一系列的数值，例如上述你想要的整数。

```py
my_integers = [1, 2, 3, 4, 5]
```

It is really simple. We created an array and stored it on  **my\_integer**.真的很简单——我们创建了一个数组（Array），并把它存在了**my\_integer**当中。

But maybe you are asking: “How can I get a value from this array?”现在你可能要问了：怎样才可以从Array中取一个数值呢？

Great question.  `List`  has a concept called  **index**. The first element gets the index 0 (zero). The second gets 1, and so on. You get the idea.问得好。List中有个概念，叫index。List中的第一个元素为index 0，第二个是index 1，依次类推。明白了吧。

To make it clearer, we can represent the array and each element with its index. I can draw it:更简单来说，我们可以用index来指代array中的每个元素。

![](https://cdn-media-1.freecodecamp.org/images/1*ReMk6NgghLII20vPD6uNEA.jpeg)

Using the Python syntax, it’s also simple to understand:Python句法比较容易理解：

```py
my_integers = [5, 7, 1, 3, 4]
print(my_integers[0]) # 5
print(my_integers[1]) # 7
print(my_integers[4]) # 4
```

Imagine that you don’t want to store integers. You just want to store strings, like a list of your relatives’ names. Mine would look something like this:如果不需要储存整数，需要储存字符串，比如要储存亲戚的名字，我家的亲戚名字如下：

```py
relatives_names = [
  "Toshiaki",
  "Juliana",
  "Yuji",
  "Bruno",
  "Kaio"
]

```

It works the same way as integers. Nice.跟储存整数一样。不错吧。

We just learned how  `Lists`  indices work. But I still need to show you how we can add an element to the  `List`  data structure (an item to a list).我们刚学习了list中的各个元素如何工作。但我还需要告诉你们如何向list数据结构中添加元素（向list中添加一个事项）。

The most common method to add a new value to a  `List`  is  `append`. Let’s see how it works:最常见的方法是运用append函数。我们一起来看看如何运用append函数。

```py
bookshelf = []
bookshelf.append("The Effective Engineer")
bookshelf.append("The 4 Hour Work Week")
print(bookshelf[0]) # The Effective Engineer
print(bookshelf[1]) # The 4 Hour Work Week
```

`append`  is super simple. You just need to apply the element (eg. “**The Effective Engineer**”) as the  `append`  parameter.append特别简单，只需要将元素添加为append的参数（正如“**The Effective Engineer**”）。

Well, enough about  `Lists`**_._**  Let’s talk about another data structure.有关list的知识就说到这里。我们一起来看看另外一个数据结构。

### Dictionary: Key-Value Data Structure字典（Dictioary）：Key-Value（键-值）数据结构

Now we know that  `Lists`  are indexed with integer numbers. But what if we don’t want to use integer numbers as indices? Some data structures that we can use are numeric, string, or other types of indices.现在我们知道list用整数来索引。但是，如果我们不想用整数来索引呢？那我们可以使用其他的数据结构，例如数值，字符串等来进行索引。

Let’s learn about the  `Dictionary`  data structure.  `Dictionary`  is a collection of key-value pairs. Here’s what it looks like:我们一起来学习一下字典（Dictionary）数据结构。Dictionary使用key-value（键-值）存储。具体使用方法如下：

```py
dictionary_example = {
  "key1": "value1",
  "key2": "value2",
  "key3": "value3"
}
```

The  **key**  is the index pointing to the **value**. How do we access the  `Dictionary`  **value**? You guessed it — using the  **key**. Let’s try it:元素key指向value。那运用key，就可以得到dictionary中的value。让我们试一下。

```py
dictionary_tk = {
  "name": "Leandro",
  "nickname": "Tk",
  "nationality": "Brazilian"
}

```

I created a  `Dictionary`  about me. My name, nickname, and nationality. Those attributes are the  `Dictionary`  **keys**.我创建了一个关于我的Dictionary，包括我的名字、绰号和国籍。这些属性就是Dictionary中的key。

As we learned how to access the  `List`  using index, we also use indices (**keys**  in the  `Dictionary`  context) to access the  **value**  stored in the  `Dictionary`.我们刚已经学过了如何运用索引得到list中的值，那我们也可以运用索引（即Dictionary中的key）来得到Dictionary中value的存放位置。

In the example, I printed a phrase about me using all the values stored in the  `Dictionary`. Pretty simple, right?例子当中，我用存储在Dictionary中的value输出了一个关于我的短语。很简单吧~

Another cool thing about  `Dictionary`  is that we can use anything as the value. In the  `Dictionary`  I created, I want to add the  **key**  “age” and my real integer age in it:Dictionary还有一个很酷的属性，就是value的值可变。在我创建的Dictionary中，我想要增加我的年龄“age”作为一个key，并且输入我年龄的整数值。

```py
dictionary_tk = {
  "name": "Leandro",
  "nickname": "Tk",
  "nationality": "Brazilian",
  "age": 24
}

```

Here we have a  **key**  (age)  **value**  (24) pair using string as the  **key**  and integer as the  **value**.现在key-value值当中，key是字符串，value是整数。

As we did with  `Lists`, let’s learn how to add elements to a  `Dictionary`. The  **key** pointing to a **value**  is a big part of what  `Dictionary`  is. This is also true when we are talking about adding elements to it:跟list一样，现在我们要学习如何向Dictionary中增加元素。key指向value是Dictionary的一大组成。向Dictionary中增加元素时也是如此。

```py
dictionary_tk = {
  "name": "Leandro",
  "nickname": "Tk",
  "nationality": "Brazilian"
}
dictionary_tk['age'] = 24

```

We just need to assign a  **value**  to a  `Dictionary` **key**. Nothing complicated here, right?我们只需要在Dictionary中设定一个value，并且对应一个key就可以了。不复杂吧。

### Iteration: Looping Through Data Structures迭代：数据结构中的循环

As we learned in the  [**Python Basics**][1], the  `List`  iteration is very simple. We  `Python`  developers commonly use  `For`  looping. Let’s do it:正如我们在Python基础中学到的内容，list迭代非常简单。我们些用Python来开发的程序员通常使用for循环。一起来做：

```py
bookshelf = [
  "The Effective Engineer",
  "The 4-hour Workweek",
  "Zero to One",
  "Lean Startup",
  "Hooked"
]

```

So for each book in the bookshelf, we (**can do everything with it**) print it. Pretty simple and intuitive. That’s Python.所以我们输出了书架上的每一本书（但我们能做的远不止于此）。这就是Python——相当简单且足够直观。

For a hash data structure, we can also use the  `for`  loop, but we apply the  `key`  :对于哈希数据结构而言，我们也可以使用for循环，但同时我们应该用到key：

```py
dictionary = { "some_key": "some_value" }
for key in dictionary:
    print("%s --> %s" %(key, dictionary[key]))

```

This is an example how to use it. For each  `key`  in the  `dictionary`  , we  `print`  the  `key`  and its corresponding  `value`.这个例子就解释了如何在for循环中使用key。我们可以输出Dictionary中的每个key以及其对应的value。

Another way to do it is to use the  `iteritems`  method.另外一个方法是使用iteritems。

```py
dictionary = { "some_key": "some_value" }
for key, value in dictionary.items():
    print("%s --> %s" %(key, value))

```

We did name the two parameters as  `key`  and  `value`, but it is not necessary. We can name them anything. Let’s see it:我们将这两个参数命名为key和value，但这并不必须。我们也可以有其他命名。比如说：

```py
dictionary_tk = {
  "name": "Leandro",
  "nickname": "Tk",
  "nationality": "Brazilian",
  "age": 24
}
for attribute, value in dictionary_tk.items():
    print("My %s is %s" %(attribute, value))

```

We can see we used attribute as a parameter for the  `Dictionary`  `key`, and it works properly. Great!可以看到，例子中我们将参数命名为attribute，替代了key，代码同样运行流畅。真棒！

### Classes & Objects类和对象

#### A little bit of theory:理论先导：

**Objects**  are a representation of real world objects like cars, dogs, or bikes. The objects share two main characteristics:  **data**  and  **behavior**.对象代表了真实世界当中的实体，例如汽车、狗狗、自行车等。这些对象有两个主要特点：数据和行为。

Cars have  **data,**  like number of wheels, number of doors, and seating capacity They also exhibit  **behavior**: they can accelerate, stop, show how much fuel is left, and so many other things.汽车包含有数据，比如轮胎数量，车门数量，和座位数量。汽车也有一定行为，例如他们可以加速，可以停下，可以显示还剩多少燃油，诸如此类。

We identify  **data**  as  **attributes**  and  **behavior**  as  **methods**  in object-oriented programming. Again:在面向对象的程序设计中，我们将数据看做属性，将行为看做方法。

Data → Attributes and Behavior → Methods数据→属性&行为→方法

And a  **Class**  is the blueprint from which individual objects are created. In the real world, we often find many objects with the same type. Like cars. All the same make and model (and all have an engine, wheels, doors, and so on). Each car was built from the same set of blueprints and has the same components.类从对象中抽象而来。真实世界当中，一种类型下有很多物体，比如汽车。所有汽车的制作过程基本一致，设计模型也相差无几，都有引擎、轮胎等等。每辆汽车都是同一批设计图纸的产物，有着相同的零部件。

#### Python Object-Oriented Programming mode: ONPython面向对象的程序设计模式：ON

Python, as an Object-Oriented programming language, has these concepts:  **class**  and  **object**.面向对象的程序设计语言——Python，有类和对象这两个概念。

A class is a blueprint, a model for its objects.类就是对象的模板，是对对象的抽象。

So again, a class it is just a model, or a way to define  **attributes**  and  **behavior**  (as we talked about in the theory section). As an example, a vehicle  **class**  has its own  **attributes**  that define what  **objects** are vehicles. The number of wheels, type of tank, seating capacity, and maximum velocity are all attributes of a vehicle.所以，类就是一种模型，一种定义属性和行为的方式（正如理论部分所讲）。举个例子，车辆这种类就有它自己的属性，属性能够定义什么对象是车辆。轮胎的数量，油箱类型，座位数量，最快速度等等，都是车辆的属性。

With this in mind, let’s look at Python syntax for  **classes**:有了这些前提，我们一起来看看Python中类的表达句法：

```py
class Vehicle:
    pass
```

We define classes with a  **class statement —** and that’s it. Easy, isn’t it?我们用类语句来定义类。

**Objects**  are instances of a  **class**. We create an instance by naming the class.对象是类的实体，是类的表现形式。通过命名类，我们可以创建实体。

```py
car = Vehicle()
print(car) # <main.Vehicle instance at 0x7fb1de6c2638>
```

Here  `car`  is an  **object**  (or instance) of the  **class**  `Vehicle`.这里的car就是“Vehicle”类中的一个对象。

Remember that our vehicle  **class**  has four  **attributes**: number of wheels, type of tank, seating capacity, and maximum velocity. We set all these  **attributes**  when creating a vehicle  **object**. So here, we define our  **class**  to receive data when it initiates it:记住，我们的“Vehicle”类中有四个属性：车轮数量，邮箱类型，座位数量和最快速度。创建一种车辆对象时我们便设置好这些属性。所以这里，一开始我们就定义类来接收数据。

```py
class Vehicle:
    def init(self, number_of_wheels, type_of_tank, seating_capacity, maximum_velocity):
        self.number_of_wheels = number_of_wheels
        self.type_of_tank = type_of_tank
        self.seating_capacity = seating_capacity
        self.maximum_velocity = maximum_velocity
```

We use the  `init`  **method**. We call it a constructor method. So when we create the vehicle  **object**, we can define these  **attributes**. Imagine that we love the  **Tesla Model S,**  and we want to create this kind of  **object**. It has four wheels, runs on electric energy, has space for five seats, and the maximum velocity is 250km/hour (155 mph). Let’s create this  **object:**我们运用了'init'方法这种构造方法。所以创建车辆对象时，我们可以定义这些属性。设想，我们喜欢**Tesla Model S,**，自然而然我们便想创建这样一种对象。这个对象有四个车轮，用电驱动前行，有四个座位，最高时速可达250km，合每小时155英里。那我们就来创建这个对象：

```py
tesla_model_s = Vehicle(4, 'electric', 5, 250)
```

Four wheels + electric “tank type” + five seats + 250km/hour maximum speed.属性包括四个车轮，用电驱动，五个车座，最高时速为250km。

All attributes are set. But how can we access these attributes’ values? We  **send a message to the object asking about them**. We call it a  **method**. It’s the  **object’s behavior**. Let’s implement it:所有属性都已经设置完毕。但是我们怎么获得这些属性的值呢？这就需要“向对象发送一条信息询问”，我们把这一过程称为“方法”，也就是“对象的行为”。我们来做一下：

```py
class Vehicle:
    def init(self, number_of_wheels, type_of_tank, seating_capacity, maximum_velocity):
        self.number_of_wheels = number_of_wheels
        self.type_of_tank = type_of_tank
        self.seating_capacity = seating_capacity
        self.maximum_velocity = maximum_velocity
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">number_of_wheels</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">return</span> self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>number_of_wheels

<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">set_number_of_wheels</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> number<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>number_of_wheels <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> number</code></pre><p style="box-sizing: inherit; margin: 0px 0px 1.5em; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; min-width: 100%;">This is an implementation of two methods:<span> </span><strong style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: bold; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; color: rgb(27, 27, 50);">number_of_wheels</strong><span> </span>and<span> </span><strong style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: bold; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; color: rgb(27, 27, 50);">set_number_of_wheels</strong>. We call it<span> </span><code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">getter</code><span> </span>&amp;<span> </span><code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">setter</code>. Because the first gets the attribute value, and the second sets a new value for the attribute.</p><p style="box-sizing: inherit; margin: 0px 0px 1.5em; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; min-width: 100%;">In Python, we can do that using<span> </span><code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">@property</code><span> </span>(<code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">decorators</code>) to define<span> </span><code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">getters</code><span> </span>and<span> </span><code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">setters</code>. Let’s see it with code:</p><pre class=" language-py" style="box-sizing: inherit; margin: 1.5em 0px 3em; padding: 20px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: 1.5em; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: 1.4rem; vertical-align: baseline; color: rgb(27, 27, 50); background: rgb(238, 238, 240); text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none; overflow: auto; min-width: 100%; max-width: 100%;"><code class=" language-py" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: inherit; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: inherit; vertical-align: baseline; color: rgb(0, 0, 0); background: transparent; text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none;"><span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">class</span> <span class="token class-name" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">Vehicle</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">__init__</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> number_of_wheels<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> type_of_tank<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> seating_capacity<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> maximum_velocity<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>number_of_wheels <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> number_of_wheels
    self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>type_of_tank <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> type_of_tank
    self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>seating_capacity <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> seating_capacity
    self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>maximum_velocity <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> maximum_velocity

@<span class="token builtin" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">property</span>
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">number_of_wheels</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">return</span> self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>__number_of_wheels

@number_of_wheels<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>setter
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">number_of_wheels</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> number<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>__number_of_wheels <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> number</code></pre><p style="box-sizing: inherit; margin: 0px 0px 1.5em; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; min-width: 100%;">And we can use these methods as attributes:</p><pre class=" language-py" style="box-sizing: inherit; margin: 1.5em 0px 3em; padding: 20px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: 1.5em; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: 1.4rem; vertical-align: baseline; color: rgb(27, 27, 50); background: rgb(238, 238, 240); text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none; overflow: auto; min-width: 100%; max-width: 100%;"><code class=" language-py" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: inherit; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: inherit; vertical-align: baseline; color: rgb(0, 0, 0); background: transparent; text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none;">tesla_model_s <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> Vehicle<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span><span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">4</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token string" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">'electric'</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">5</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">250</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span>
```

This is slightly different than defining methods. The methods work as attributes. For example, when we set the new number of wheels, we don’t apply two as a parameter, but set the value 2 to  `number_of_wheels`. This is one way to write  `pythonic`  `getter`  and  `setter`  code.这个跟定义“方法”不太一样。这种情况下，“方法”作为参数运转。举个例子，设定车轮数量时，我们不是把“2”作为参数，而是把“2”赋值给“车轮数量”这一属性。而这也是写pythonic，getter和setter代码的一种方法。

But we can also use methods for other things, like the “**make\_noise**” method. Let’s see it:当然“方法”也有其他用途，以“**make\_noise**”方法为例：
```py
class Vehicle:
    def init(self, number_of_wheels, type_of_tank, seating_capacity, maximum_velocity):
        self.number_of_wheels = number_of_wheels
        self.type_of_tank = type_of_tank
        self.seating_capacity = seating_capacity
        self.maximum_velocity = maximum_velocity
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">make_noise</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">print</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span><span class="token string" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">'VRUUUUUUUM'</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span></code></pre><p style="box-sizing: inherit; margin: 0px 0px 1.5em; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; min-width: 100%;">When we call this method, it just returns a string<span> </span><strong style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: bold; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; color: rgb(27, 27, 50);"><em style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: italic; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; color: rgb(27, 27, 50);">“</em>VRRRRUUUUM.<em style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: italic; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; color: rgb(27, 27, 50);">”</em></strong></p><pre class=" language-py" style="box-sizing: inherit; margin: 1.5em 0px 3em; padding: 20px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: 1.5em; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: 1.4rem; vertical-align: baseline; color: rgb(27, 27, 50); background: rgb(238, 238, 240); text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none; overflow: auto; min-width: 100%; max-width: 100%;"><code class=" language-py" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: inherit; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: inherit; vertical-align: baseline; color: rgb(0, 0, 0); background: transparent; text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none;">tesla_model_s <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> Vehicle<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span><span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">4</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token string" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">'electric'</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">5</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">250</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span>
```

### Encapsulation: Hiding Information封装：隐藏信息

Encapsulation is a mechanism that restricts direct access to objects’ data and methods. But at the same time, it facilitates operation on that data (objects’ methods).封装机制限制对象数据和方法的直接访问。但同时，封装有利于数据（对象的方法）层面的操作。

> “Encapsulation can be used to hide data members and members function. Under this definition, encapsulation means that the internal representation of an  [object][2]  is generally hidden from view outside of the object’s definition.” — Wikipedia维基百科上说：“封装可以用来隐藏数据成员和成员函数。封装意味着对象的内部实现通常被隐藏，并由定义替代。”

All internal representation of an object is hidden from the outside. Only the object can interact with its internal data.对象的左右内部实现都被隐藏，只有对象本身可以和内部数据互动。

First, we need to understand how  `public`  and  `non-public`  instance variables and methods work.首先，我们需要理解公共(public)和非公共(non-public)实例变量以及方法是如何工作。

#### Public Instance Variables公共实例变量

For a Python class, we can initialize a  `public instance variable`  within our constructor method. Let’s see this:对于Python当中的类而言，我们在构造方法中预置一个公共实例变量，如下：

Within the constructor method:在构造方法内部：

```py
class Person:
    def init(self, first_name):
        self.first_name = first_name
```

Here we apply the  `first_name`  value as an argument to the  `public instance variable`.我们将"first_name"的值赋给公共实例变量。

```py
tk = Person('TK')
print(tk.first_name) # => TK
```

Within the class:在类当中，如果我们直接给first_name定义：

```py
class Person:
    first_name = 'TK'
```

Here, we do not need to apply the  `first_name`  as an argument, and all instance objects will have a  `class attribute`  initialized with  `TK`.那我们就不需要再给变量赋值，因为所有的实例对象都会有初始化的类属性——"TK".

```py
tk = Person()
print(tk.first_name) # => TK
```

Cool. We have now learned that we can use  `public instance variables`  and  `class attributes`. Another interesting thing about the  `public`  part is that we can manage the variable value. What do I mean by that? Our  `object`  can manage its variable value:  `Get`  and  `Set`  variable values.现在我们已经学过了如何使用公共实例变量和类属性。公共实例变量还有一个特点，就是可变。什么意思呢？就是我们的对象可以通过"Get"和"Set"变量值来管理自身变量值。

Keeping the  `Person`  class in mind, we want to set another value to its  `first_name`  variable:脑子里想象一个"Person"类，我们想要给这个类当中的"first_name"变量设定一个值：

```py
tk = Person('TK')
tk.first_name = 'Kaio'
print(tk.first_name) # => Kaio
```

There we go. We just set another value (`kaio`) to the  `first_name`  instance variable and it updated the value. Simple as that. Since it’s a  `public`  variable, we can do that.我们将"Kaio"赋值给"first_name"这个实例变量，实例变量随之更新。原因就在于，这是一个公共变量。

#### Non-public Instance Variable非公共实例变量

> We don’t use the term “private” here, since no attribute is really private in Python (without a generally unnecessary amount of work). —  [PEP 8][3]因为Python（没有一大堆不必要的工作时）[3]当中没有一个变量完全私有不公开，所以我们这里使用了非公共(non-public)这个词，而没用使用私有(private)这个词。

As the  `public instance variable`  , we can define the  `non-public instance variable`  both within the constructor method or within the class. The syntax difference is: for  `non-public instance variables`  , use an underscore (`_`) before the  `variable`  name.跟公共实例变量无异，我们也可以在构造方法和类当中定义非公共实例变量。句法差异在于：对于非公共实例变量而言，需要在变量名字前使用"_".

> “‘Private’ instance variables that cannot be accessed except from inside an object don’t exist in Python. However, there is a convention that is followed by most Python code: a name prefixed with an underscore (e.g.  `_spam_`_) should be treated as a non-public part of the API (whether it is a function, a method or a data member)” —  [Python Software Foundation][4]_根据Python软体基金会，“Python中不存在私有实例变量，除了在对象内部，否则不能得到私有实例变量。然而，Python中大多数代码都遵循一条惯例：无论是函数、方法或者数据成员，只有其名字前有一条下划线（例如"_spam_"_），它就可以被视为API（应用编程接口）的非公共部分。”

_Here’s an example:_例子如下：

_`class Person:
    def __init_`_`(self, first_name, email):
        self.first_name = first_name
        self._email = email_`

_Did you see the  `email`  variable? This is how we define a  `non-public variable`  :_看见"email"变量了吧，这就是定义非公共变量的方式。

_`tk = Person('TK', 'tk@mail.com')
print(tk._email) # [tk@mail.com][5]_`_

> __We can access and update it.  `Non-public variables`  are just a convention and should be treated as a non-public part of the API.__

__So we use a method that allows us to do it inside our class definition. Let’s implement two methods (`email`  and  `update_email`) to understand it:__我们可以获得并且更新非公共变量。非公共变量只是一种约定俗成，不应被当做API的非公共部分。所以我们采用一种方法，可以让我们在类的定义中将非公共变量当做非公共部分。两个方法("email" & "update_email")可帮助理解：

__`class Person:
    def __init`__`(self, first_name, email):
        self.first_name = first_name
        self._email = email

```
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">update_email</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> new_email<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>_email <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> new_email

<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">email</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">return</span> self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>_email</code></pre><p style="box-sizing: inherit; margin: 0px 0px 1.5em; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; min-width: 100%;">Now we can update and access<span> </span><code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">non-public variables</code><span> </span>using those methods. Let’s see:</p><pre class=" language-py" style="box-sizing: inherit; margin: 1.5em 0px 3em; padding: 20px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: 1.5em; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: 1.4rem; vertical-align: baseline; color: rgb(27, 27, 50); background: rgb(238, 238, 240); text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none; overflow: auto; min-width: 100%; max-width: 100%;"><code class=" language-py" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: inherit; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: inherit; vertical-align: baseline; color: rgb(0, 0, 0); background: transparent; text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none;">tk <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> Person<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span><span class="token string" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">'TK'</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token string" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">'tk@mail.com'</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span>
```

`

`print(tk.email()) # => [tk@mail.com][6]
# tk._email = 'new_tk@mail.com' -- treat as a non-public part of the class API_ _print(tk.email()) # => [tk@mail.com][7]
tk.update_email('new_tk@mail.com')
print(tk.email()) # => [new_tk@mail.com][8]_`

1.  _We initiated a new object with  `first_name`  TK and  `email`  [tk@mail.com][9]_我们引入了一个新对象，包括"first_name"和"email"。
2.  _Printed the email by accessing the  `non-public variable`  with a method_我们用一种方法得到了非公共变量，输出了"email"。
3.  _Tried to set a new  `email`  out of our class_我们试图在类之外设置一个新的"email"。
4.  _We need to treat  `non-public variable`  as  `non-public`  part of the API_我们需要将非公共变量视作API的非公共部分。
5.  _Updated the  `non-public variable`  with our instance method_运用实例方法更新了非公共变量。
6.  _Success! We can update it inside our class with the helper method_大功告成！可运用助手方法(the helper method)在类中更新。

#### _Public Method_公共方法

_With  `public methods`, we can also use them out of our class:_公共方法也可以在类之外使用。

_`class Person:
    def __init_`_`(self, first_name, age):
        self.first_name = first_name
        self._age = age

```
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">show_age</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">return</span> self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>_age</code></pre><p style="box-sizing: inherit; margin: 0px 0px 1.5em; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; min-width: 100%;">我们来测试一下：</p><pre class=" language-py" style="box-sizing: inherit; margin: 1.5em 0px 3em; padding: 20px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: 1.5em; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: 1.4rem; vertical-align: baseline; color: rgb(27, 27, 50); background: rgb(238, 238, 240); text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none; overflow: auto; min-width: 100%; max-width: 100%;"><code class=" language-py" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: inherit; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: inherit; vertical-align: baseline; color: rgb(0, 0, 0); background: transparent; text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none;">tk <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> Person<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span><span class="token string" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">'TK'</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">25</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span>
```

`

`print(tk.show_age()) # => 25`

Great — we can use it without any problem.棒极了！这样用没有任何问题。

#### Non-public Method非公共方法

But with  `non-public methods`  we aren’t able to do it. Let’s implement the same  `Person`  class, but now with a  `show_age`  `non-public method`  using an underscore (`_`).非公共方法无法在类之外使用。我们要用到同一个"Person"类，用下划线表示添加非公共方法"show_age"。

```py
class Person:
    def init(self, first_name, age):
        self.first_name = first_name
        self._age = age
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">_show_age</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">return</span> self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>_age</code></pre><p style="box-sizing: inherit; margin: 0px 0px 1.5em; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; min-width: 100%;">And now, we’ll try to call this<span> </span><code style="box-sizing: inherit; margin: 0px; padding: 0px 5px 2px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: 1em; font-family: &quot;Roboto Mono&quot;, monospace; font-size: 0.8em; vertical-align: baseline; background: rgb(208, 208, 213); word-break: break-all;">non-public method</code><span> </span>with our object:</p><pre class=" language-py" style="box-sizing: inherit; margin: 1.5em 0px 3em; padding: 20px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: 1.5em; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: 1.4rem; vertical-align: baseline; color: rgb(27, 27, 50); background: rgb(238, 238, 240); text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none; overflow: auto; min-width: 100%; max-width: 100%;"><code class=" language-py" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: 400 !important; font-stretch: inherit; line-height: inherit; font-family: Consolas, Monaco, &quot;Andale Mono&quot;, &quot;Ubuntu Mono&quot;, monospace; font-size: inherit; vertical-align: baseline; color: rgb(0, 0, 0); background: transparent; text-shadow: rgb(255, 255, 255) 0px 1px; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; overflow-wrap: normal; tab-size: 4; hyphens: none;">tk <span class="token operator" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(154, 110, 58);">=</span> Person<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span><span class="token string" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(102, 153, 0);">'TK'</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">,</span> <span class="token number" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 0, 85);">25</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span>
```

> _We can access and update it.  `Non-public methods`  are just a convention and should be treated as a non-public part of the API._我们可以得到并且更新非公共方法。这一方法是一个惯例，应该被视为API中的非公共部分。

_Here’s an example for how we can use it:_下面的例子显示了非公共方法的使用过程：

_`class Person:
    def __init_`_`(self, first_name, age):
        self.first_name = first_name
        self._age = age

```
<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">show_age</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">return</span> self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>_get_age<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span>

<span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">def</span> <span class="token function" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(221, 74, 104);">_get_age</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">(</span>self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">)</span><span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">:</span>
    <span class="token keyword" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(0, 119, 170);">return</span> self<span class="token punctuation" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 15px; vertical-align: baseline; color: rgb(153, 153, 153);">.</span>_age
```

`

`tk = Person('TK', 25)
print(tk.show_age()) # => 25`

Here we have a  `_get_age_` _`non-public method`  and a  `show_age`  `public method`. The  `show_age`  can be used by our object (out of our class) and the  `_get_age_` _only used inside our class definition (inside  `show_age`  method). But again: as a matter of convention.__这里我们既有非公共方法"_get_age_"，也有公共方法"show_age"。"show_age"可以在类之外由我们的对象使用，但是"_get_age_"只能在类定义（"show_age"方法之内）之内使用。需再次强调，非公共方法是一种约定俗成。

#### __Encapsulation Summary__封装总结

__With encapsulation we can ensure that the internal representation of the object is hidden from the outside.__封装可以确保对象的内部实现被隐藏。

### __Inheritance: behaviors and characteristics__继承：行为和特点

__Certain objects have some things in common: their behavior and characteristics.__特定对象的共同点在于他们的行为和特点。

__For example, I inherited some characteristics and behaviors from my father. I inherited his eyes and hair as characteristics, and his impatience and introversion as behaviors.__比如说，我继承了我父亲的一些特点和行为。特点方面，我有跟父亲一样的大眼睛和头发；行为方面，我跟父亲一样缺乏耐心，性格内向。

__In object-oriented programming, classes can inherit common characteristics (data) and behavior (methods) from another class.__在面向对象的程序设计中，类可以从其他的类中继承共同的特点（即数据）和行为（即方法）。

__Let’s see another example and implement it in Python.__下面这个例子可以用在Python中。

__Imagine a car. Number of wheels, seating capacity and maximum velocity are all attributes of a car. We can say that an  **ElectricCar** class inherits these same attributes from the regular  **Car**  class.__想象有一辆汽车。汽车的属性包括车轮数量、车座个数和最高时速。那“电动汽车”类就可以从常规“汽车”类继承一些相同的属性。

__`class Car:
    def __init_`_`(self, number_of_wheels, seating_capacity, maximum_velocity):
        self.number_of_wheels = number_of_wheels
        self.seating_capacity = seating_capacity
        self.maximum_velocity = maximum_velocity`_

_Our  **Car**  class implemented:_我们的“汽车”类就可以直接使用这些：

_`my_car = Car(4, 5, 250)
print(my_car.number_of_wheels)
print(my_car.seating_capacity)
print(my_car.maximum_velocity)`_

_Once initiated, we can use all  `instance variables`  created. Nice._开始后，我们就可以使用所有创建好的“实例变量”。

_In Python, we apply a  `parent class`  to the  `child class`  as a parameter. An  **ElectricCar**  class can inherit from our  **Car**  class._Python中，我们将父类作为参数应用到子类中，好比“电动汽车”类可以从“车类”继承行为和特点。

_`class ElectricCar(Car):
    def **init**(self, number_of_wheels, seating_capacity, maximum_velocity):
        Car.**init**(self, number_of_wheels, seating_capacity, maximum_velocity)`_

_Simple as that. We don’t need to implement any other method, because this class already has it (inherited from  **Car**  class). Let’s prove it:_不难吧。因为从“车”类继承过来的方法，我们无需在使用其他任何方法。验证一下：

_`my_electric_car = ElectricCar(4, 5, 250)
print(my_electric_car.number_of_wheels) # => 4
print(my_electric_car.seating_capacity) # => 5
print(my_electric_car.maximum_velocity) # => 250`_

_Beautiful._一个字：爽！

### _That’s it!_大概就这么多。

_We learned a lot of things about Python basics:_总结一下我们学习的Python基础知识：

-   _How Python variables work_变量如何工作
-   _How Python conditional statements work_条件语句
-   _How Python looping (while & for) works_while & for循环
-   _How to use Lists: Collection | Array_列表：集合|数组
-   _Dictionary Key-Value Collection_字典键-值集合
-   _How we can iterate through these data structures_如何在数据结构中迭代
-   _Objects and Classes_对象和类
-   _Attributes as objects’ data_属性作为对象数据
-   _Methods as objects’ behavior_方法作为对象行为
-   _Using Python getters and setters & property decorator_Python中的getters setters和property decorator
-   _Encapsulation: hiding information_封装：隐藏信息
-   _Inheritance: behaviors and characteristics_继承：行为和特点

_Congrats! You completed this dense piece of content about Python._祝贺你！你已经完成这一部分的Python学习！

_If you want a complete Python course, learn more real-world coding skills and build projects, try  [**One Month Python Bootcamp_**][10]. See you there ☺_如果你想学习一套完整的Python课程，学习更多的编程技巧，搭建项目，试着点击[**One Month Python Bootcamp_**]。期待看见你的身影~

_For more stories and posts about my journey learning & mastering programming, follow my publication  [**The Renaissance Developer**][11]._想了解更多我的编程学习历程，可以关注我的网站[**The Renaissance Developer**]

_Have fun, keep learning, and always keep coding._终身学习，坚持编程，笑口常开。

_My  <a href="[https://twitter.com/LeandroTk][12]_" rel="noopener" style="box-sizing: inherit; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-size: 22px; vertical-align: baseline; background-color: transparent; color: rgb(10, 10, 35); text-decoration: underline; cursor: pointer; word-break: break-word;">Twitter  &  [Github][13]. ☺欢迎关注我的Twitter[https://twitter.com/LeandroTk]和GitHub[https://github.com/LeandroTk]账号。

[1]: https://medium.com/the-renaissance-developer/python-101-the-basics-441136fb7cc3
[2]: https://en.wikipedia.org/wiki/Object_(computer_science)
[3]: https://www.python.org/dev/peps/pep-0008/#designing-for-inheritance
[4]: https://docs.python.org/2/tutorial/classes.html#private-variables-and-class-local-references
[5]: mailto:tk@mail.com
[6]: mailto:tk@mail.com
[7]: mailto:tk@mail.com
[8]: mailto:new_tk@mail.com
[9]: mailto:tk@mail.com
[10]: https://onemonth.com/courses/python?campaignid=33447&discount_code=TKPython1&mbsy=lG6tv&mbsy_source=7d89eeb0-0031-478c-a60c-6a96d762712a
[11]: https://medium.com/the-renaissance-developer
[12]: https://twitter.com/LeandroTk
[13]: https://github.com/LeandroTk