> php是一门计算机编程语言，主要应用于开发web应用(网站建设等)，本系列博客从php基础语法出发，介绍php基础知识。使读者深入浅出的学习到编程的乐趣。
> 
> 本系列博客将讲解以下9个知识点，**变量、常量、数据类型、运算符、数组、流程控制(顺序、选择、循环)、函数、文件处理、面向对象**
> 
> 每篇文章都会在文末留下一个课后作业，答案获取请私聊我，大家可以在评论区积极讨论，共同进步


![函数](https://img-blog.csdnimg.cn/20210419141429419.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3JlYmVrYWhf,size_16,color_FFFFFF,t_70)

# 概念
不管学习什么样的编程语言，函数都是必不可少的一个点。函数为什么这么重要呢？是因为使用函数可以减少代码的冗余度，提升代码的复用性。大大增加编程的效率。所以我们一定要认真学习它。

首先，什么是函数？函数就是将一段相关的代码块封装起来并且赋予它一个专门的名字。在其他地方，我们只需要叫它的名字即可完成调用。

举一个生活中的例子，我们去饭店吃饭需要首先点菜， 比如点一个青椒肉丝，老板只需要对后厨喊一声青椒肉丝，具体的细节他并不用关心。后厨在听到青椒肉丝后，将完成切菜、准备食材、炒菜、装盘、上菜等操作。

在这个例子中，后厨的种种行为就是函数体(也就是一段相关的代码块)，函数名也就是青椒肉丝，老板喊一声青椒肉丝也就是在调用函数。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
/**
 * 青椒肉丝(函数)
 */
function qingjiaorousi() 
{
    printf("切菜");
    echo "<br />";
    printf("准备食材");
    echo "<br />";
    printf("炒菜");
    echo "<br />";
    printf("装盘");
    echo "<br />";
    printf("上菜");
    echo "<br />";
}
qingjiaorousi(); //调用函数
```

# 函数的格式
`function 函数名(形参)
{
	函数体
	return xx; //返回值
}`

注：
	1、申明函数必须以funtion为开头 ，函数名一般不重复；
	2、形参可以有也可以不用
	3、返回值可以没有，如果有必唯一。

# 代码实操
编写一个a+b的函数，并且用一个变量接收返回值并输出。请用代码实现。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

//add函数功能为a+b
function add($a, $b)
{
    $sum = $a + $b;
    return $sum;
}

$c = add(10 , 20);
echo $c;
```
执行结果：
![函数](https://img-blog.csdnimg.cn/2021041914073818.png)


# 课后练习
1、函数是什么？如何申明函数？


2、编写一个a-b的函数，并且用一个变量接收返回值并输出。请用代码实现。



> 课后练习答案，通过微信搜一搜「 学长冷月 」回复**php**获取
> 文章持续更新，本文 GitHub [https://github.com/lengyueit/phpFamily](https://github.com/lengyueit/phpFamily) 已收录，欢迎Star。