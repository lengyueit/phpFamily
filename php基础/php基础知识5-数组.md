> php是一门计算机编程语言，主要应用于开发web应用(网站建设等)，本系列博客从php基础语法出发，介绍php基础知识。使读者深入浅出的学习到编程的乐趣。
> 
> 本系列博客将讲解以下9个知识点，**变量、常量、数据类型、运算符、数组、流程控制(顺序、选择、循环)、函数、文件处理、面向对象**
> 
> 每篇文章都会在文末留下一个课后作业，答案获取请私聊我，大家可以在评论区积极讨论，共同进步

![数组](https://img-blog.csdnimg.cn/img_convert/5772b65decec14158dafada0164560b5.png)

# 概念
在学习了**变量和常量**之后，我们发现不管是变量和常量都只能存储一个数据。

那么我们想象一个场景，假如一个学习小组有5位同学，我们要存储这5位同学的名字。不管是变量还是常量都不太适合运用于这个场景。这时候我们就引入了数组的概念。

数组是一个能在单个变量中存储多个值的特殊变量。一般将一组相关联的数据存储在一个数组中。

数组示例：

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$arr = [1,2,3,4,5]; //数组$arr存储了1,2,3,4,5
```

**数组定义方式**

 - 使用`[]`的方式
$arr = [1,2,3,4,5];

 - 使用array()函数
$arr = array(1,2,3,4,5);


# 分类
 - **索引数组**
定义数组时直接输入值，按`,`分割，自动生成索引（从0开始）。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$arr = ["xiaoming","xiaobai","lengyue"]; //定义数组$arr
var_dump($arr); //输出$arr
```
![索引数组](https://img-blog.csdnimg.cn/img_convert/4819fb3a89000d16d21a61a7d36a2756.png)

 - **关联数组**
定义时需要指定的键，每个键关联一个值。语法格式如下所示：

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$arr = [
    "name" => "lengyue",
    "age" => 22,
    "country" => "China"
];
var_dump($arr);
```
![关联数组](https://img-blog.csdnimg.cn/img_convert/be6aff3cc6e25282b4d899d75019838b.png)
 - **二维数组**
一维数组只能定义了一个人的某些属性（姓名，年龄，国家）。那么如果我们有多个人怎么办呢？二维数组也就派上了用场。
二维数组就相当于是一个表格。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$arr = [
    [
        "name" => "lengyue",
        "age" => 22,
        "country" => "China"
    ],
    [
        "name" => "xiaohong",
        "age" => 20,
        "country" => "USA"
    ],
    [
        "name" => "tony",
        "age" => 35,
        "country" => "China"
    ],
];
var_dump($arr);
```
![二维数组](https://img-blog.csdnimg.cn/img_convert/a6768a38ef79622cb1024bde0c7c5034.png)

# 代码实操
将以下表格中的数据使用合适的数组形式，用代码实现出来：
![数组实例](https://img-blog.csdnimg.cn/img_convert/776dc063675c1122e7e0680e040cd238.png)

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$arr = array(
    array("10点","语文","张老师"),
    array("11点","数学","王老师"),
    array("12点","英语","李老师"),
);
var_dump($arr);
```

![实例结果](https://img-blog.csdnimg.cn/img_convert/e2ad700f9cb2a0fca7acf234a41122d0.png)

# 课后练习

 1. 数组是什么？分为哪几类？

 2. `array("10点","语文","张老师")`这是索引数组还是关联数组？



> 课后练习答案，通过微信搜一搜「 学长冷月 」回复**php**获取
> 文章持续更新，本文 GitHub [https://github.com/lengyueit/phpFamily](https://github.com/lengyueit/phpFamily) 已收录，欢迎Star。