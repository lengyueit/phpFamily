> php是一门计算机编程语言，主要应用于开发web应用(网站建设等)，本系列博客从php基础语法出发，介绍php基础知识。使读者深入浅出的学习到编程的乐趣。
> 
> 本系列博客将讲解以下9个知识点，**变量、常量、数据类型、运算符、数组、流程控制(顺序、选择、循环)、函数、文件处理、面向对象**
> 
> 每篇文章都会在文末留下一个课后作业，答案获取请私聊我，大家可以在评论区积极讨论，共同进步


![流程控制](https://img-blog.csdnimg.cn/20210418223443928.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3JlYmVrYWhf,size_16,color_FFFFFF,t_70)

# 概念
简单来说流程控制决定代码的执行顺序，在实际编程中，莫过于顺序、选择、循环这三种场景，我们将这三种场景学会后，就可以读懂大多数的代码。

对于初学者而言，流程控制是一大难点。但是却是不可缺少的一部分。我们要认真的学习它。
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          
# 顺序结构
顺序结构顾名思义是顺序执行的，换句话来说代码从上往下依次执行，不会跳过中间的某一行代码。平时编程大多数代码都是顺序结构。

# 选择结构
选择结构有点像高中数学里学习的程序框图里面的分支结构，也就是说满足条件则这段代码，不满足条件则执行另一段代码。同时也可以嵌套其他的语句。php 里面主要是以if...else...、switch...case...等为主。

**if...else...**
如果if后面的表达式成立则执行第一个大括号的语句，否则执行第二个大括号的语句。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
if (2>1) {
    echo "2大于1";
} else {
    echo "2不大于1";
}
```
执行结果：
![流程控制](https://img-blog.csdnimg.cn/20210418195834539.png)

**if...elseif...else**
如果if后面的表达式成立则执行第一个大括号的语句，然后判断elseif的语句是否成立，若成立则执行第二个大括号的语句，否则执行第三个大括号的语句。并且可以继续嵌套。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
if (2 > 1) {
    echo "2大于1";
} elseif (1 > 0) {
    echo "1大于0";
} else {
    echo "1不大于0";
}
```
执行结果：
![流程控制](https://img-blog.csdnimg.cn/20210418195834539.png)

**switch...case...**
根据switch后面的大括号的值进行 每一个case块的匹配，匹配成功则执行相应的大括号的语句。

注：
**每一个case块最后必须加上break; 否则一旦匹配成功，将会将后面的所有代码执行，包括其他case块的代码。**

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$month = 4;
switch ($month)
{
    case 1:
        echo "1月";
        break;
    case 2:
        echo "2月";
        break;
    case 3:
        echo "3月";
        break;
    case 4:
        echo "4月";
        break;
    case 5:
        echo "5月";
        break;
    case 6:
        echo "6月";
        break;
    case 7:
        echo "7月";
        break;
    case 8:
        echo "8月";
        break;
    case 9:
        echo "9月";
        break;
    case 10:
        echo "10月";
        break;
    case 11:
        echo "11月";
        break;
    case 12:
        echo "12月";
        break;
}
```

执行结果：
![流程控制](https://img-blog.csdnimg.cn/20210418200739358.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3JlYmVrYWhf,size_16,color_FFFFFF,t_70)

# 循环结构
如果有业务场景是需要重复执行一段代码，则循环结构是二不之选。

**for**

for循环格式：`for(表达式1;表达式2;表达式3){代码块}`

表达式1给控制变量赋初值，表达式2为设置跳出条件，表达式3为步长。
```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

for ($i = 0; $i < 10; $i++) {
    printf("我要买{$i}杯牛奶");
    echo "<br />";
}
```
执行结果：
![流程控制](https://img-blog.csdnimg.cn/2021041820155029.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3JlYmVrYWhf,size_16,color_FFFFFF,t_70)
**while**

while循环格式：`while(表达式){代码块}`
如果while的条件为永真，则会一直执行，陷入死循环；如果为永假，则一次也不执行。
```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

$i = 0;
while ($i<10)
{
    printf("我要买{$i}杯牛奶");
    echo "<br />";
    $i++;
}
```
执行结果：
![流程控制](https://img-blog.csdnimg.cn/2021041820155029.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3JlYmVrYWhf,size_16,color_FFFFFF,t_70)
**do .. while**

do..while循环格式：`do{代码块}while(表达式)`
如果while的条件为永真，则会一直执行，陷入死循环；如果为永假，则也会执行一次。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */

$i = 10; //给$i 赋初值为10
do {
    printf("我要买{$i}杯牛奶");
    echo "<br />";
    $i++; 
} while ($i < 10); //$i不小于10 条件为假
```
执行结果：

![流程控制](https://img-blog.csdnimg.cn/20210418202859831.png)
# 代码实操
业务场景:小明期末考试不及格，回到家后，如果首先告诉爸爸则会被打10下手掌；如果首先告诉妈妈则会被罚跑5圈步。请用合适的代码表示出来。

```php
<?php
/**
 * Created by 冷月小白.
 * 微信公众号: 学长冷月
 */
$i = 1; //用1代表告诉爸爸
switch ($i) {
    case 1: //用1代表告诉爸爸
        for ($j = 1; $j <= 10; $j++) {
            printf("被打的第{$j}下手掌");
            echo "<br />";
        }
        break;
    case 2: //用2代表告诉妈妈
        for ($j = 1; $j <= 5; $j++) {
            printf("被罚跑的第{$j}圈");
            echo "<br />";
        }
        break;
}
```
执行结果：
![流程控制](https://img-blog.csdnimg.cn/2021041821511765.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3JlYmVrYWhf,size_16,color_FFFFFF,t_70)

# 课后练习

1、while 和do...while的区别


2、业务场景:小明期末考试考了68分，之前和爸爸约定只要诚实的说出分数，则无论如何都可以去一次游乐园之后每多10分就可以多去一次，请用合适的代码表示出来。

> 课后练习答案，通过微信搜一搜「 学长冷月 」回复**php**获取
> 文章持续更新，本文 GitHub [https://github.com/lengyueit/phpFamily](https://github.com/lengyueit/phpFamily) 已收录，欢迎Star。