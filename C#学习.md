##### C#访问修饰符

public : 同一程序集的其他任何代码或引用该程序集的其他程序集都可以访问该类型或成员。
internal : 同一程序集中的任何代码都可以访问该类型或成员，但其他程序集不可以访问。
private : 同一类和结构的代码可以访问该类型和成员。
protected : 同一类和派生(继承特性)类中的代码可以访问该类型和成员。
protected internal :  同一程序集中的任何代码或其他程序集中的任何派生类都可以访问该类型或成员。
private protected：该类型或成员可以通过从 class 派生的类型访问，这些类型在其包含程序集中进行声明
![image-20240116153715060](C#知识点_markdown_image/image-20240116153715060.png)

(1) 类、结构的默认修饰符是internal。
(2) 类中所有的成员默认修饰符是private。
(3) 接口默认修饰符是internal。
(4) 接口的成员默认修饰符是public。
(5) 枚举类型成员默认修饰符是public。
(6) 委托的默认修饰符是internal。


