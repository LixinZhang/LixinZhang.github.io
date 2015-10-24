Title: C++概念重载、覆盖、隐藏
Date: 2011-06-12 06:00
Author: 糖拌咸鱼
Slug: cgai-nian-zhong-zai-fu-gai-yin-cang

函数重载:

</p>

在C++程序中，可以将语义、功能相似的几个函数用同一个名字表示，即函数重载。

</p>

重载的实现:

</p>

几个同名的重载函数仍然是不同的函数，它们是如何区分的呢？我们自然想到函数接口的两个要素：参数与返回值。如果同名函数的参数不同（包括类型、顺序不同），那么容易区别出它们是不同的函数。

</p>

重载与覆盖成员函数被重载的特征：

</p>

（1）相同的范围（在同一个类中）；

</p>

（2）函数名字相同；

</p>

（3）参数不同；

</p>

（4）virtual 关键字可有可无。

</p>

覆盖是指派生类函数覆盖基类函数，特征是：

</p>

（1）不同的范围（分别位于派生类与基类）；

</p>

（2）函数名字相同；

</p>

（3）参数相同；

</p>

（4）基类函数必须有virtual 关键字。

</p>

隐藏规则:本来仅仅区别重载与覆盖并不算困难，但是C++的隐藏规则使问题复杂性增加了许多。这里“隐藏”是指派生类的函数屏蔽了与其同名的基类函数，规则如下：

</p>

（1）如果派生类的函数与基类的函数同名，但是参数不同。此时，不论有无virtual关键字，基类的函数将被隐藏（注意别与重载混淆）。

</p>

（2）如果派生类的函数与基类的函数同名，并且参数也相同，但是基类函数没有virtual关键字。此时，基类的函数被隐藏（注意别与覆盖混淆）。

</p>
