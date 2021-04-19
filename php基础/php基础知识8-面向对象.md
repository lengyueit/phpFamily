> php是一门计算机编程语言，主要应用于开发web应用(网站建设等)，本系列博客从php基础语法出发，介绍php基础知识。使读者深入浅出的学习到编程的乐趣。
> 
> 本系列博客将讲解以下9个知识点，**变量、常量、数据类型、运算符、数组、流程控制(顺序、选择、循环)、函数、文件处理、面向对象**
> 
> 每篇文章都会在文末留下一个课后作业，答案获取请私聊我，大家可以在评论区积极讨论，共同进步

![面向对象](https://img-blog.csdnimg.cn/20210419160541214.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3JlYmVrYWhf,size_16,color_FFFFFF,t_70)
# 概念
前面我们所学习到的知识大多都是面向过程的编程方式。相信大家再开始学习编程知识后，经常听到类、对象这些术语。其实这些都是面向对象的相关知识。我们简单的介绍一下面向对象的知识来作为我们这个系列博客的收尾。

在进一步学习面向对象之前呢，我们首先要对编程思想做一个转变。将某些相关的代码抽象为类，增强代码的复用性。

# 类
我们可以将类理解为一个抽象的事物，对象理解为对具体事物的描写。这句话理解起来可能有些抽象。下面我们举一个例子来帮助大家理解。

世界上的人可以分为男人和女人，也可以分为老人、青年、小孩。那么我们可以将所有的人都抽象为一个类。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

class Person
{
    public $sex; //性别

    //睡觉方法
    public function sleep()
    {
        echo "睡觉";
    }
    
    //吃饭方法
    public function eat()
    {
        echo "吃饭";
    }
}
```
在类里面，我们可以声明属性和方法。属性其实就是变量，方法其实就是函数。

# 对象
在构造了一个类之后，我们要怎么使用它呢？可以通过实例化对象的方式，也就是常听说的new一个对象。请看下面这段代码：

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

class Person
{
    public $sex; //性别

    //睡觉方法
    public function sleep()
    {
        echo $this->sex."睡觉";
        echo "<br />";
    }

    //吃饭方法
    public function eat()
    {
        echo $this->sex."吃饭";
        echo "<br />";
    }
}

$manObj = new Person(); //实例化对象
$manObj->sex = "男"; //修改成员属性sex为男
$manObj->sleep(); //调用成员方法sleep
$manObj->eat();//调用成员方法eat
```

输出结果：
![面向对象](https://img-blog.csdnimg.cn/20210419160334956.png)

也就是说我们可以通过实例化对象，然后对这个对象进行定制化的操作，以达到代码复用的目的。

最后，相信大家已经对于php中的面向对象已经有了一定的了解，但是这还远远不够，希望大家进一步的学习，争取早日成为大牛。

# 课后练习
1、类和对象的区别。


2、请编写一个Dog类，包括eat()和sleep()两个方法。并实例化输出。


> 课后练习答案，通过微信搜一搜「 学长冷月 」回复**php**获取
> 文章持续更新，本文 GitHub [https://github.com/lengyueit/phpFamily](https://github.com/lengyueit/phpFamily) 已收录，欢迎Star。