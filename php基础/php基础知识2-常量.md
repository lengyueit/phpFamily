> php是一门计算机编程语言，主要应用于开发web应用(网站建设等)，本系列博客从php基础语法出发，介绍php基础知识。使读者深入浅出的学习到编程的乐趣。
> 
> 本系列博客将讲解以下9个知识点，**变量、常量、数据类型、运算符、数组、流程控制(顺序、选择、循环)、函数、文件处理、面向对象**
> 
> 每篇文章都会在文末留下一个课后作业，答案获取请私聊我，大家可以在评论区积极讨论，共同进步


![常量导学](https://img-blog.csdnimg.cn/img_convert/c06b705466ca1baab3124241d505110f.png)
# 常量的概念
常量顾名思义是不变的量，在整个php代码执行阶段其值不能改变。

常量的命名规则同变量一样，但是传统上常量标识符总是大写的。并且常量的声明不用加$符号。

初学的小伙伴肯定会认为变量和常量都是代表一个值，那么为啥还要区分变量和常量呢？其实变量和常量都各自不用的职责，在真实开发中会根据不同的使用场景来选择合适的变量和常量。

**如何申明常量**

 - define()函数
使用php内置的define()即可定义常量，第一个参数为常量名(大写)，第二个参数为常量值。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
define("NAME","lengyue");  //NAME为常量名 ， lengyue为值
echo NAME; //输出lengyue
```

 - 使用const关键字
直接在声明常量前加关键字 `const`即可。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
const NAME = "lengyue";
echo NAME;
```

# 代码实操

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

define("NAME","lengyue"); //使用define()声明常量NAME
echo NAME;
const AGE = 18;//使用const声明常量AGE
echo AGE;
```


# 课后练习

 1. 声明常量的两种方法？

 2. 常量的命名规则？



> 课后练习答案，通过微信搜一搜「 学长冷月 」回复**php**获取
> 文章持续更新，本文 GitHub [https://github.com/lengyueit/phpFamily](https://github.com/lengyueit/phpFamily) 已收录，欢迎Star。