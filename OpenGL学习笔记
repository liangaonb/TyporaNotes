# OpenGL

- #### 关于CMake

<img src="OpenGL学习笔记_markdown_image/image-20240222105046430.png" alt="image-20240222105046430" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240222110103955.png" alt="image-20240222110103955" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240222124503377.png" alt="image-20240222124503377" style="zoom:80%;" />

如果分享给其他人，需要删除.vs和out文件夹（这些文件可以使用CMake自动生成）

<img src="OpenGL学习笔记_markdown_image/image-20240222125409993.png" alt="image-20240222125409993" style="zoom:80%;" />

. SRCS中的.是当前CMakeLists.txt所在目录的意思。${SRCS}是将SRCS中的内容取出，即{"main.cpp" "func.cpp"}。

编译和链接。编译只检查你使用的函数是否声明过（.h），而链接则会检查你使用的函数是否实现了(.cpp)。

.lib是静态链接库，.dll是动态链接库。

![image-20240222132951956](OpenGL学习笔记_markdown_image/image-20240222132951956.png)

![image-20240222142617872](OpenGL学习笔记_markdown_image/image-20240222142617872.png)

![image-20240222143416264](OpenGL学习笔记_markdown_image/image-20240222143416264.png)

<img src="OpenGL学习笔记_markdown_image/image-20240223125447046.png" alt="image-20240223125447046" style="zoom:80%;" />

为了在include的时候不用写全路径，可以在CMakeLists中增加如下指令：

![image-20240223124343164](OpenGL学习笔记_markdown_image/image-20240223124343164.png)

<img src="OpenGL学习笔记_markdown_image/image-20240223124755480.png" alt="image-20240223124755480" style="zoom:67%;" />

为了能够链接所需要的lib文件，还需要添加如下指令：

<img src="OpenGL学习笔记_markdown_image/image-20240223125301138.png" alt="image-20240223125301138" style="zoom:80%;" />

对于glad的配置，为了将glad.c加入到编译中，修改指令如下：

<img src="OpenGL学习笔记_markdown_image/image-20240225194723322.png" alt="image-20240225194723322" style="zoom:80%;" />

在include时，glad.h要在glfw3.h之前：

<img src="OpenGL学习笔记_markdown_image/image-20240227134819413.png" alt="image-20240227134819413" style="zoom:80%;" />

在有主CMakeLists和子CMakeLists的情况下，

这是子CMakeLists：

<img src="OpenGL学习笔记_markdown_image/image-20240301200421958.png" alt="image-20240301200421958" style="zoom:80%;" />

这是主CMakeLists：

<img src="OpenGL学习笔记_markdown_image/image-20240301201351676.png" alt="image-20240301201351676" style="zoom:80%;" />

然后在链接的时候添加进去即可：

<img src="OpenGL学习笔记_markdown_image/image-20240301200658642.png" alt="image-20240301200658642" style="zoom:80%;" />

- #### 基础窗体搭建

<img src="OpenGL学习笔记_markdown_image/image-20240227132042971.png" alt="image-20240227132042971" style="zoom:80%;" />

每次循环称为一帧，可以在循环中使用OpenGL渲染场景。

- #### 事件响应

<img src="OpenGL学习笔记_markdown_image/image-20240227192235311.png" alt="image-20240227192235311" style="zoom:80%;" />

- #### 函数加载

<img src="OpenGL学习笔记_markdown_image/image-20240227201844180.png" alt="image-20240227201844180" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240227203940660.png" alt="image-20240227203940660" style="zoom:80%;" />

- #### GL函数初体验

<img src="OpenGL学习笔记_markdown_image/image-20240227204532823.png" alt="image-20240227204532823" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240227204803762.png" alt="image-20240227204803762" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240227205125446.png" alt="image-20240227205125446" style="zoom:80%;" />

- #### OpenGL错误检查

<img src="OpenGL学习笔记_markdown_image/image-20240229150129250.png" alt="image-20240229150129250" style="zoom:80%;" />

- #### 应用层--Application单例类设计

<img src="OpenGL学习笔记_markdown_image/image-20240304165446584.png" alt="image-20240304165446584" style="zoom:80%;" />

Application表示应用程序本身，全局只能有一个对象，所以要用单例模式。

<img src="OpenGL学习笔记_markdown_image/image-20240304165930031.png" alt="image-20240304165930031" style="zoom:80%;" />

- #### Application成员变量与成员函数设计

<img src="OpenGL学习笔记_markdown_image/image-20240305141151535.png" alt="image-20240305141151535" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240305141335915.png" alt="image-20240305141335915" style="zoom:80%;" />

- #### Application事件回调

<img src="OpenGL学习笔记_markdown_image/image-20240305184625617.png" alt="image-20240305184625617" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240305190750029.png" alt="image-20240305190750029" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240305190932029.png" alt="image-20240305190932029" style="zoom:80%;" />

- #### NDC介绍

<img src="OpenGL学习笔记_markdown_image/image-20240306191431190.png" alt="image-20240306191431190" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240306191710873.png" alt="image-20240306191710873" style="zoom:80%;" />

- #### VBO介绍

<img src="OpenGL学习笔记_markdown_image/image-20240306192735954.png" alt="image-20240306192735954" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240306193109723.png" alt="image-20240306193109723" style="zoom:80%;" />

- #### VBO绑定与数据传输

<img src="OpenGL学习笔记_markdown_image/image-20240306195117274.png" alt="image-20240306195117274" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240306195542512.png" alt="image-20240306195542512" style="zoom:80%;" />

- #### VBO多属性数据

<img src="OpenGL学习笔记_markdown_image/image-20240307135608731.png" alt="image-20240307135608731" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307142840799.png" alt="image-20240307142840799" style="zoom:80%;" />

- #### VAO介绍

<img src="OpenGL学习笔记_markdown_image/image-20240307144224829.png" alt="image-20240307144224829" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307151308379.png" alt="image-20240307151308379" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307151453098.png" alt="image-20240307151453098" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307151652361.png" alt="image-20240307151652361" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307153055577.png" alt="image-20240307153055577" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307153212339.png" alt="image-20240307153212339" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307153414690.png" alt="image-20240307153414690" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240307153641417.png" alt="image-20240307153641417" style="zoom:80%;" />

- #### VAO搭建之SingleBuffer

<img src="OpenGL学习笔记_markdown_image/image-20240312130839908.png" alt="image-20240312130839908" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312131957393.png" alt="image-20240312131957393" style="zoom:80%;" />

- #### VAO搭建之InterleavedBuffer

<img src="OpenGL学习笔记_markdown_image/image-20240312135933816.png" alt="image-20240312135933816" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312140153431.png" alt="image-20240312140153431" style="zoom:80%;" />

- #### VBO、VAO总结

<img src="OpenGL学习笔记_markdown_image/image-20240312145123970.png" alt="image-20240312145123970" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312145146046.png" alt="image-20240312145146046" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312145401148.png" alt="image-20240312145401148" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312145550104.png" alt="image-20240312145550104" style="zoom:80%;" />

- #### Shader介绍

<img src="OpenGL学习笔记_markdown_image/image-20240312145914316.png" alt="image-20240312145914316" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312150045451.png" alt="image-20240312150045451" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312150439092.png" alt="image-20240312150439092" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312150741019.png" alt="image-20240312150741019" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312151117986.png" alt="image-20240312151117986" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240312151449671.png" alt="image-20240312151449671" style="zoom:80%;" />

- #### shader的编译与链接

<img src="OpenGL学习笔记_markdown_image/image-20240312193138767.png" alt="image-20240312193138767" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240318201354731.png" alt="image-20240318201354731" style="zoom:80%;" />

- #### glDrawArray绘制命令

<img src="OpenGL学习笔记_markdown_image/image-20240318202924318.png" alt="image-20240318202924318" style="zoom:80%;" />

<img src="OpenGL学习笔记_markdown_image/image-20240318203026929.png" alt="image-20240318203026929" style="zoom:80%;" />

- #### 多顶点数据绘制

<img src="OpenGL学习笔记_markdown_image/image-20240318210321881.png" alt="image-20240318210321881" style="zoom:80%;" />

- #### 绘制命令+绘制模式
