> php是一门计算机编程语言，主要应用于开发web应用(网站建设等)，本系列博客从php基础语法出发，介绍php基础知识。使读者深入浅出的学习到编程的乐趣。
> 
> 本系列博客将讲解以下9个知识点，**变量、常量、数据类型、运算符、数组、流程控制(顺序、选择、循环)、函数、文件处理、面向对象**
> 
> 每篇文章都会在文末留下一个课后作业，答案获取请私聊我，大家可以在评论区积极讨论，共同进步



![数据类型导学](https://img-blog.csdnimg.cn/img_convert/61b8ff55a23e74252f8e3930b7425fce.png)

# 数据类型的概念
很多初学的小伙伴对于数据类型这一定义很难理解，其实如果给出一个数，计算机并不像人一样能够一眼识别出是整数还是小数，计算机只能识别0 和 1的二进制代码，而数据类型就是帮助计算机识别这个数到底是整数还是小数。

本文将介绍php中5大基础数据类型：`int(整型)、float（浮点型）、string（字符串类型）、bool（布尔类型）、null`（空类型）
# 数据类型的分类

 - int(整型)
int(整型)，其实就是整数，像100、-50 这样不带小数的整数都叫整型，可以是正数或负数。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

$a = 100;
$b = -50;
```

 - float（浮点型）
float（浮点型），其实就是小数，像10.05、2.03 这样带小数都叫浮点型

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

$a = 10.05;
$b = 2.03;
```

 - string（字符串类型）
string（字符串类型），顾名思义就是一段字符串例如 `"abc"或者'abc'`，用单引号和双引号包含都可。
输出字符串要用var_dump()函数。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

$a = "i am lengyue";
$b = 'my name is lengyue';

var_dump($a); //打印i am lengyue
var_dump($b);//my name is lengyue
```

 - bool（布尔类型）
 布尔型通常用于条件判断。可以是 TRUE(真) 或 FALSE(假)。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$a = true; //真
$b = false; //假
```

 - null（空类型）
NULL 值表示变量没有值。NULL 是数据类型为 NULL 的值。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$a = null; //数据为空
```
# 代码实操

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
//int
$a = 100; //  100
$b = -50;//  -50

//float
$a = 10.05;//  10.05
$b = 2.03;//  2.03

//string
$a = "i am lengyue";
$b = 'my name is lengyue';

//bool
$a = true; //真
$b = false; //假

//null
$a = null; //数据为空
```

# 课后练习

1. php中数据类型有哪些？分别怎么定义？


 2. 字符串类型中 `'' 和 ""`  有什么区别？



> 课后练习答案，通过微信搜一搜「 学长冷月 」回复**php**获取
> 文章持续更新，本文 GitHub [https://github.com/lengyueit/phpFamily](https://github.com/lengyueit/phpFamily) 已收录，欢迎Star。