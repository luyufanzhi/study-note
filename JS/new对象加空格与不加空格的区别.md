# new一个对象后面加括号与不加括号的区别

&nbsp;

## 加括号与不加的区别

（1）加括号

	1. 若括号为空，即无实参项，那么理解为调用默认构造函数；
 	2. 若括号非空，即有实参项，可以理解为调用重载构造函数，或    复合默认构造函数。

（2）不加括号

　	调用默认构造函数，或复合默认构造函数。



## 默认构造函数 与 复合默认构造函数的区别 ##
**默认构造函数**：编译器会为每一个类默认提供一个构造函数，称之为默认构造函数。默认构造函数一般参数为空。

**复合默认构造函数**：一个由用户自定义的所有形式参数都赋有默认值的构造函数，称之为复合默认构造函数。



**两者联系**：

一个类中，若一旦有一个用户自定义构造函数，那么由编译器提供的默认构造函数就不再存在。用户自定义的构造函数为默认构造函数的重载版。

默认构造函数不复存在时，用户必须为这个类再自定义一个复合默认构造函数（选所有自定义构造函数其中之一，把形式参数均赋默认值即可）。

不论自定义构造函数（即构造函数的重载版）有多少个，只允许有一个复合默认构造函数。