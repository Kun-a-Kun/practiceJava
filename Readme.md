# Java从入门到入土
## 语法
* for-each循环
使用`Employee e`遍历`staff`数组
```java
Employee[] staff=new Employee[3];
        staff[0]=new Employee("",9000,1999,1,1);
        staff[1]=new Employee("little B",10000,1999,2,2);
        staff[2]=new Employee("little C",12000,1999,3,3);

        for(Employee e:staff)
            e.raiseSalary(5);
```
## 对象与类
* private成员变量的访问只有在类的内部可以访问，
限定是类。同一个类的不同对象之间可以访问别人的私有成员。
私有针对类，不针对对象。
例：[翁凯java第一周编程题（58行）](File://C:\Users\Administrator\Desktop\practiceJava\moocJavaWengKai\src\fraction\Fraction.java)中plus()中的r.c。
* 如果要接受一个对象引用作为构造器参数，要考虑是否能接受可有可无
的值。例：[java核心技术p110 4.3.6null（28行）](File://C:\Users\Administrator\Desktop\practiceJava\coreJavaVolume\src\EmployeeTest.java)

宽容型：`Object.requireNonNulllElse()`  
严格型：`Object.requireNonNull()`

* 如何写出良好的代码(可扩展性，封装等)参考视频：[翁凯面向对象程序设计-城堡游戏](https://www.bilibili.com/video/BV1Mb411z7qx?p=32)
 相关代码：[castle](File://C:\Users\ZYY\Desktop\practiceJava\moocJavaWengKai\src\castle)
      
  
## String StringBuffer StringBuilder
简单来说，String值不可变，每次对String对象的改变都会生成新的String
对象。效率低下，浪费内存。对于经常要改变的对象来说，使用StringBuffer和StringBuilder。
具体见:[String、StringBuffer与StringBuilder之间区别](https://blog.csdn.net/itchuxuezhe_yang/article/details/89966303)