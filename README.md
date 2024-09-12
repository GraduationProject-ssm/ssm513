# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# ssm513基于VUE的图书馆管理系统的设计与实现+vue

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1t58veLEnL?p=111)


# 第1章 绪论
## 1.1 课题背景
互联网发展至今，无论是其理论还是技术都已经成熟，而且它广泛参与在社会中的方方面面。它让信息都可以通过网络传播，搭配信息管理工具可以很好地为人们提供服务。所以各行业，尤其是规模较大的企业和学校等都开始借助互联网和软件工具管理信息，传播信息，共享信息等等，以此可以增强自身实力，提高在同行业当中的竞争能力，并从各种激烈的竞争中获取发展的机会。针对购买书籍信息管理混乱，出错率高，信息安全性差，劳动强度大，费时费力等问题，经过分析和考虑，在目前的情况下，可以引进一款图书馆管理系统这样的现代化管理工具，这个工具就是解决上述问题的最好的解决方案。它不仅可以实时完成信息处理，还缩短购买书籍信息管理流程，使其系统化和规范化。同时还可以减少工作量，节约购买书籍信息管理需要的人力和资金。所以图书馆管理系统是信息管理环节中不可缺少的工具，它对管理者来说非常重要。
## 1.2 课题意义 
现如今，信息种类变得越来越多，信息的容量也变得越来越大，这就是信息时代的标志。近些年，计算机科学发展得也越来越快，而且软件开发技术也越来越成熟，因此，在生活中的各个领域，只要存在信息管理，几乎都有计算机的影子，可以说很多行业都采用计算机的方式管理信息。信息计算机化处理相比手工操作，有着保密性强，效率高，存储空间大，成本低等诸多优点。针对购买书籍信息管理，采用图书馆管理系统可以有效管理，使信息管理能够更加科学和规范。

总之，在实际中使用图书馆管理系统，其意义如下：

第一点：图书馆管理系统的实际运用，可以帮助管理人员在短时间内完成信息处理工作；

第二点：通过系统页面的合理排版布局，可以更加直观的展示系统的内容，并且使用者可以随时阅读页面信息，随时操作系统提供的功能；

第三点：可以实现信息管理计算机化；

第四点：可以降低信息管理成本；
## 1.3 研究内容
对图书馆管理系统设计制作，不仅需要技术支撑，也需要大量的理论研究。本文在对图书馆管理系统进行介绍时，将按照如下内容进行。

第一部分：介绍图书馆管理系统研究的背景意义，便于用户了解系统；

第二部分：介绍开发图书馆管理系统需要搭建的环境，包括技术和工具；

第三部分：介绍用户对图书馆管理系统的功能要求，以及对图书馆管理系统的性能要求等；

第四部分：介绍数据库的设计方案，以及根据功能要求设计的功能结构；

第五部分：介绍通过编码最终实现的系统功能运行效果；

第六部分：介绍系统的功能测试，对系统进行综合检测，并及时解决系统出现的问题，直至系统运行正常。
# 第2章 开发环境与技术
图书馆管理系统的编码实现需要搭建一定的环境和使用相应的技术，接下来的内容就是对图书馆管理系统用到的技术和工具进行介绍。
## 2.1 MYSQL数据库
本课题所开发的应用程序在数据操作方面是不可预知的，是经常变动的，没有办法直接把数据写在文档里，这样不仅仅不安全，也不能实现应用程序的功能。如果要能实现应用程序所需要的数据存储功能，就避免不了要进行专业数据库存储软件的选择。基本上应用程序实现的功能不算太复杂，市面上任何一个关系型数据库软件都可以实现。参考自己的学习进度和操作习惯来讲，Oracle数据库是适合的，但是所需要的的安装软件很大，并且有好多不需要的功能都是开启的状态，十分消耗电脑资源，所以没有选择Oracle数据库，而SQL Server数据库虽然学过，但是安装的时候因为电脑上可能有其他的软件存在，经常性的出问题，而安装问题不好解决就需要重新安装操作系统，这样对已经存在的软件来讲又是一种时间上的浪费。只有MySQL数据库，安装包小，安装速度快，操作简单，哪怕安装出问题也好解决，不用重装操作系统，也不影响电脑上运行的其他软件，消耗资源也少，最重要的是在功能方面完全的符合设计需要，所以最后选择了MySQL数据库作为应用软件开发需要的数据库。
## 2.2 vue技术  
在动态网站的兴起之初，作为高级编程语言的Java自然不会放弃这个领域的蛋糕。Sun公司推出了Servlet作为输出动态网站的一种技术标准，虽然不怎么受当时程序员的喜爱，但是当初也没有太多的选择，随后几个月java语言问世，不考虑性能和效率如何，起码在书写网页所需要的动态代码块和静态代码块方面进行了区分，让书写效率和可读效率大大的提升，所以很多Java程序员以及刚入行的初级程序员都选择了java语言作为自己职业的发展方向，Sun公司为了维护Java语言在高级编程语言上的江湖地位，防止java继续抢走市场份额占有率，Sun公司联合Apache基金会研发了一个关于Java动态网页的一个新型的技术标准，这就是vue技术。vue吸取了java语言在页面书写上面的所有优点，但是又背靠Java EE的庞大后台，又能实现很多通过Java组件就能实现的功能，在vue页面上可以直接引用那些组件，让vue更加的强壮丰富。保证了Java技术纵向的可持续发展，并且在动态网站开发领域终于站稳了脚跟，其他java开发人员可以很快的转移到vue进行开发，不考虑一些特殊组件或者功能的开发，只从动态页面的开发上来讲，完全实现了java程序和vue程序的几乎无成本的转换，vue技术就这样的发展了起来。
## 2.3 Spring Boot框架
Spring Boot是由Pivotal团队提供的全新[框架](https://baike.baidu.com/item/%E6%A1%86%E6%9E%B6/1212667)，其设计目的是用来[简化](https://baike.baidu.com/item/%E7%AE%80%E5%8C%96/3374416)新[Spring](https://baike.baidu.com/item/Spring/85061)应用的初始搭建以及开发过程。该框架使用了特定的方式来进行配置，从而使开发人员不再需要定义样板化的配置。通过这种方式，Spring Boot致力于在蓬勃发展的快速应用开发领域(rapid application development)成为领导者。

` `SpringBoot基于Spring4.0设计，不仅继承了Spring框架原有的优秀特性，而且还通过简化配置来进一步简化了Spring应用的整个搭建和开发过程。另外SpringBoot通过集成大量的框架使得依赖包的版本冲突，以及引用的不稳定性等问题得到了很好的解决。

SpringBoot框架中还有两个非常重要的策略：开箱即用和约定优于配置。开箱即用，Outofbox，是指在开发过程中，通过在MAVEN项目的pom文件中添加相关依赖包，然后使用对应注解来代替繁琐的XML配置文件以管理对象的生命周期。这个特点使得开发人员摆脱了复杂的配置工作以及依赖的管理工作，更加专注于业务逻辑。约定优于配置，Convention over configuration，是一种由SpringBoot本身来配置目标结构，由开发者在结构中添加信息的软件设计范式。这一特点虽降低了部分灵活性，增加了BUG定位的复杂性，但减少了开发人员需要做出决定的数量，同时减少了大量的XML配置，并且可以将代码编译、测试和打包等工作自动化。

SpringBoot应用系统开发模板的基本架构设计从前端到后台进行说明：前端常使用模板引擎，主要有FreeMarker和Thymeleaf，它们都是用Java语言编写的，渲染模板并输出相应文本，使得界面的设计与应用的逻辑分离，同时前端开发还会使用到Bootstrap、AngularJS、JQuery等；在浏览器的数据传输格式上采用Json，非xml，同时提供RESTfulAPI；SpringMVC框架用于数据到达服务器后处理请求；到[数据访问层](https://baike.baidu.com/item/%E6%95%B0%E6%8D%AE%E8%AE%BF%E9%97%AE%E5%B1%82/7279662)主要有Hibernate、MyBatis、JPA等持久层框架；数据库常用[MySQL](https://baike.baidu.com/item/MySQL/471251)；开发工具推荐IntelliJIDEA。
# 第3章 系统分析
面对即将开发的系统，进行提前的分析是必要的。这也是开发流程中必须有的环节。通常分析系统期间，主要涉及的内容包括系统开发可行性问题，对系统功能和性能的分析等问题。
## 3.1 可行性分析
在正式对需要建设的项目进行投资前，有一个比较关键的步骤是不能缺少的，那就是可行性分析。它主要从当前技术，经济等角度去评估系统的可行性，在投资决策中常常采用这种科学的方法来论证项目。
### 3.1.1 技术可行性
当前，系统开发的技术已经发展成熟，而且通过计算机网络可以获取开发工具的使用方法，以及规范化编写的模块化代码，这些知识可以帮助开发者顺利完成本系统的编码工作。
### 3.1.2 经济可行性
本系统开发期间需要配置的软件环境，可以免费通过开发类官网下载安装，需要配置的硬件设备也不需要具备很高的性能，通常网吧电脑，或学校计算机机房的电脑都符合要求。因此，从经济方面考虑，图书馆管理系统开发可行。
### 3.1.3 操作可行性
图书馆管理系统根据用户使用习惯进行开发，设计的界面具有统一性，并具备优秀的导航功能。所以，只要会简单操作电脑的人员，可以无压力操作图书馆管理系统。

总之，从上述的论证来看，本系统可以开发。
## 3.2 系统流程
流程图这样的工具可以直观反映出系统内部的操作逻辑，可以帮助用户更好的理解系统。
### 3.2.1 操作流程
进入本系统需要访问者提供验证信息。验证合格的访问者才能获取访问资格。其具体的操作流程见下图。访问者根据登录界面设置的信息项如实填写，待信息通过验证后，访问者可以进入指定的页面享受本系统提供的服务和阅读本系统的相关信息。

![](/md/blog.001.png)

图3.1 操作流程图
### 3.2.2 登录流程
本系统的登录模块，其内部的流程见下图。主要对访问本系统的人员提供的验证信息进行逐个判断，系统面对录入错误的信息会给出提示，比如，提示账号不对，或提示密码不匹配等提示信息。总之，在登录页面填写的所有信息都符合要求，访问者就登录成功了。

![](/md/blog.002.png)

图3.2 登录流程图
### 3.2.3 删除信息流程
本系统在经常性的使用后，会产生很多失去价值的信息，因此就需要及时清理数据，腾出系统的空间。对这些数据进行清理时，其对应的流程见下图。先选中要清理的数据，通过反复确认需要清理的数据，避免操作人员误删。已经删除的数据就不会出现在系统里面。

![](/md/blog.003.png)

图3.3 删除信息流程图
### 3.2.4 添加信息流程
本系统主要用于显示信息，提供服务，其中，数据添加功能就是其中的服务之一，具体流程见下图。让操作者在信息添加的页面录入数据，待这些数据被提交检验合格后，就会在系统指定页面显示出来。

![](/md/blog.004.png)

图3.4 添加信息流程图
## 3.3 性能需求
进行需求分析，包括了根据用户实际需求制定功能，也涵盖了对即将设计的系统进行性能上的需求分析。所以一般分析系统时，一方面要分析系统功能，另一方面也要分析系统的性能。毕竟设计开发出一个好性能的系统可以确保系统的质量可靠。

接下来分析系统的性能，还要从界面友好性，系统的时间特性，系统的可靠性等方面来分析说明。

（1）时间特性要求：系统处理数据都有时间要求，这也是系统的时间特性。通常都会把数据处理的时间进行分析，也会设置用户请求的响应时间，还有系统在满负荷运行时可以偏离的范围数值等都需要提前分析确定。

（2）界面友好性：除了功能上需要考虑用户需求外，在人机交互界面的设计上，也需要考虑用户的使用习惯，包括界面的布局，界面基调选择以及颜色搭配等。尽量做到用户在接受简单的培训之后，可以对系统进行独立操作。

（3）系统可靠性：对于初学者而言，很容易出现一个问题，就是设计开发的系统，因为人为的误操作出现崩溃，有些也会导致电脑死机。这样的现象也说明这种容错能力低下的系统是不可靠的。完全不能作为生活中处理信息的系统。当下，系统开发要保证可靠性，设计时，把模块化和结构化的设计理念也考虑进来。如果遇到对时效性要求比较严格的系统，也需要采取其它的措施，比如双机系统，还有磁盘阵列等方式。还有就是一个可靠性的系统，对设备的供电能力也有要求。
# 第4章 系统设计
一个成功设计的系统在内容上必定是丰富的，在系统外观或系统功能上必定是对用户友好的。所以为了提升系统的价值，吸引更多的访问者访问系统，以及让来访用户可以花费更多时间停留在系统上，则表明该系统设计得比较专业。
## 4.1 设计原则
本系统在设计过程中需要依照一定的设计原则进行，目的就是为了让开发的系统具备高质量，齐全完备的功能，方便简单的操作，如此才可以最大限度的满足使用者的要求。系统设计原则除了基本的易操作原则外，还有安全性原则，准确性原则。

第一个设计原则：易操作原则，针对本系统设计的功能要完备齐全，编码时，设计的各个接口要具备友好性，使用者一旦使用本系统时，要能够轻松上手，操作本系统处理数据时，要具备便利性。此外，也需要设计一些必要提示，引导使用者操作系统。

第二个设计原则：安全性原则，本系统在登录模块要对各个访问者进行身份验证，系统会通过访问者输入的信息进行判断，使用提前编写的安全验证代码进行数据比对，引导匹配成功的访问者进入指定的操作界面。这样可以避免无关性访问者窃取系统的数据。

第三个设计原则：准确性原则，为了保证使用者登记的数据是正确的，需要提前设计数据纠错机制，让使用者可以通过系统的报错提示，仔细检查登记的错误信息，并及时纠正错误，填写规范正确的信息。比如设置密码时，要求密码的长度不能低于6个字符，且数据类型要求不能全部是数字等都能进行规范。
## 4.2 功能结构设计
在前面分析的管理员功能的基础上，进行接下来的设计工作，最终展示设计的管理员结构图（见下图）。管理员增删改查购买书籍

图书馆管理系统


用户信息管理

书籍借阅管理

书籍信息管理

购买书籍管理


用户信息修改

用户信息新增

购买书籍添加 

购买书籍删除

购买书籍修改

书籍类型添加

书籍类型修改


书籍类型删除

书籍借阅添加

书籍借阅删改

书籍借阅删除

书籍信息添加 

书籍信息修改 

书籍信息删除 

书籍捐赠管理

书籍捐赠修改

书籍捐赠删除


书籍捐赠添加


书籍类型管理
## ![](/md/blog.005.png)
4.3 数据库设计

开发一个系统也需要提前设计数据库。这里的数据库是相关数据的集合，存储在一起的这些数据也是按照一定的组织方式进行的。目前，数据库能够服务于多种应用程序，则是源于它存储方式最佳，具备数据冗余率低的优势。虽然数据库为程序提供信息存储服务，但它与程序之间也可以保持较高的独立性。总而言之，数据库经历了很长一段时间的发展，从最初的不为人知，到现在的人尽皆知，其相关技术也越发成熟，同时也拥有着坚实的理论基础。

4.3.1 数据库概念设计

这部分内容需要借助数据库关系图来完成，也需要使用专门绘制数据库关系图的工具，比如Visio工具就可以设计E-R图（数据库关系图）。设计数据库，也需要按照设计的流程进行，首先还是要根据需求完成实体的确定，分析实体具有的特征，还有对实体间的关联关系进行确定。最后才是使用E-R模型的表示方法，绘制本系统的E-R图。不管是使用亿图软件，还是Visio工具，对于E-R模型的表示符号都一样，通常矩形代表实体，实体间存在的关系用菱形符号表示，实体的属性也就是实体的特征用符号椭圆表示。最后使用直线将矩形，菱形和椭圆等符号连接起来。接下来就开始对本系统的E-R图进行绘制。

（1）下图是用户实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\用户.jpg](/md/blog.006.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\用户.jpg")
图4.1 用户实体属性图

（2）下图是字典表实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\字典表.jpg](/md/blog.007.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\字典表.jpg")
图4.2 字典表实体属性图

（3）下图是购物车实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\购物车.jpg](/md/blog.008.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\购物车.jpg")
图4.3 购物车实体属性图

（4）下图是书籍信息实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍信息.jpg](/md/blog.009.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍信息.jpg")
图4.4 书籍信息实体属性图

（5）下图是书籍借阅记录实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍借阅记录.jpg](/md/blog.010.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍借阅记录.jpg")
图4.5 书籍借阅记录实体属性图

（6）下图是书籍购买实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍购买.jpg](/md/blog.011.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍购买.jpg")
图4.6 书籍购买实体属性图

（7）下图是预约书籍实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\预约书籍.jpg](/md/blog.012.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\预约书籍.jpg")
图4.7 预约书籍实体属性图

（8）下图是捐赠书籍实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\捐赠书籍.jpg](/md/blog.013.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\捐赠书籍.jpg")
图4.8 捐赠书籍实体属性图

（9）下图是书籍评价实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍评价.jpg](/md/blog.014.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍评价.jpg")
图4.9 书籍评价实体属性图

（10）下图是书籍订单实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍订单.jpg](/md/blog.015.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\书籍订单.jpg")
图4.10 书籍订单实体属性图

（11）下图是用户表实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\用户表.jpg](/md/blog.016.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\用户表.jpg")
图4.11 用户表实体属性图

（12）下图是收货地址实体和其具备的属性。

![C:\Users\Administrator\Desktop\img\tushuguanlixitong\收货地址.jpg](/md/blog.017.jpeg "C:\Users\Administrator\Desktop\img\tushuguanlixitong\收货地址.jpg")
图4.12 收货地址实体属性图
### 4.3.2 数据库物理设计
本数据库是关系型数据库，因此对二维表的结构设计也比较关键。毕竟二维表格模型就是关系型数据库中的关系模型。而一些常用的关系模型中的概念也需要了解，才可以对关系模型进行设计。下面就简单介绍关系，元组，属性，域，关键字等常用概念的含义。

关系：关系就是数据库中的一张数据表，每张数据表都有命名，也就是每个关系也有名字，那就是数据表名；

元组：元组就是数据表中的一行记录；

属性：属性就是数据表中的字段，也就是数据表中的一列；

域：域就是对数据表中属性的取值进行限定；

关键字：关键字就是数据表中的主键；

在了解了表结构设计的常用概念后，接下来就需要使用前面绘制的E-R模型完成表结构的设计工作，并在数据库中创建数据表，并为各个数据表进行命名。以下就对设计的结果通过表格形式进行展示。


表4.1收货地址表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|yonghu\_id|Integer|创建用户|是|
|3|address\_name|String|收货人|是|
|4|address\_phone|String|电话|是|
|5|address\_dizhi|String|地址|是|
|6|isdefault\_types|Integer|是否默认地址|是|
|7|insert\_time|Date|添加时间|是|
|8|update\_time|Date|修改时间|是|
|9|create\_time|Date|创建时间|是|
表4.2购物车表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|yonghu\_id|Integer|所属用户|是|
|3|shujigoumai\_id|Integer|书籍|是|
|4|buy\_number|Integer|购买数量|是|
|5|create\_time|Date|添加时间|是|
|6|update\_time|Date|更新时间|是|
|7|insert\_time|Date|创建时间|是|
表4.3字典表表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|dic\_code|String|字段|是|
|3|dic\_name|String|字段名|是|
|4|code\_index|Integer|编码|是|
|5|index\_name|String|编码名字|是|
|6|super\_id|Integer|父字段id|是|
|7|beizhu|String|备注|是|
|8|create\_time|Date|创建时间|是|
表4.4捐赠书籍表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|juanzengshuji\_name|String|书籍名称|是|
|3|juanzengshuji\_zuozhe|String|书籍作者|是|
|4|juanzengshuji\_chubanshe|String|出版社|是|
|5|shujigoumai\_types|Integer|书籍类型|是|
|6|yonghu\_id|Integer|用户|是|
|7|juanzengshuji\_time|Date|捐赠时间|是|
|8|create\_time|Date|创建时间|是|
表4.5书籍购买表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|shujigoumai\_uuid\_number|String|书籍编号|是|
|3|shujigoumai\_name|String|书籍名称|是|
|4|shujigoumai\_types|Integer|书籍类型|是|
|5|shujigoumai\_photo|String|书籍照片|是|
|6|shujigoumai\_kucun\_number|Integer|书籍库存|是|
|7|shujigoumai\_zuozhe|String|书籍作者|是|
|8|shujigoumai\_chubanshe|String|出版社|是|
|9|shujigoumai\_old\_money|BigDecimal|书籍原价|是|
|10|shujigoumai\_new\_money|BigDecimal|现价|是|
|11|shangxia\_types|Integer|是否上架|是|
|12|shujigoumai\_delete|Integer|逻辑删除|是|
|13|shujigoumai\_content|String|书籍简介|是|
|14|create\_time|Date|创建时间|是|
表4.6书籍评价表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|shujigoumai\_id|Integer|书籍|是|
|3|yonghu\_id|Integer|用户|是|
|4|shujigoumai\_commentback\_text|String|评价内容|是|
|5|reply\_text|String|回复内容|是|
|6|insert\_time|Date|评价时间|是|
|7|update\_time|Date|回复时间|是|
|8|create\_time|Date|创建时间|是|
表4.7书籍订单表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|shujigoumai\_order\_uuid\_number|String|订单号|是|
|3|shujigoumai\_id|Integer|书籍|是|
|4|yonghu\_id|Integer|用户|是|
|5|address\_id|Integer|地址|是|
|6|buy\_number|Integer|购买的数量|是|
|7|shujigoumai\_order\_true\_price|BigDecimal|实付价格|是|
|8|shujigoumai\_order\_types|Integer|订单类型|是|
|9|shujigoumai\_order\_payment\_types|Integer|支付类型|是|
|10|insert\_time|Date|订单创建时间|是|
|11|create\_time|Date|创建时间|是|
表4.8书籍借阅记录表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|shujixinxi\_id|Integer|书籍|是|
|3|yonghu\_id|Integer|用户|是|
|4|jieyue\_types|Integer|借阅状态|是|
|5|shujijieyuejie\_time|Date|借书时间|是|
|6|shujijieyuehuan\_time|Date|还书时间|是|
|7|create\_time|Date|创建时间|是|
表4.9书籍信息表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|shujixinxi\_uuid\_number|String|书籍编号|是|
|3|shujixinxi\_name|String|书籍名称|是|
|4|shujigoumai\_types|Integer|书籍类型|是|
|5|shujixinxi\_photo|String|书籍照片|是|
|6|shujixinxi\_kucun\_number|Integer|书籍库存|是|
|7|shujixinxi\_zuozhe|String|书籍作者|是|
|8|shujixinxi\_chubanshe|String|出版社|是|
|9|shujixinxi\_delete|Integer|逻辑删除|是|
|10|shujixinxi\_content|String|书籍简介|是|
|11|create\_time|Date|创建时间|是|
表4.10用户表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|yonghu\_name|String|用户姓名|是|
|3|yonghu\_photo|String|头像|是|
|4|yonghu\_phone|String|用户手机号|是|
|5|yonghu\_id\_number|String|用户身份证号|是|
|6|yonghu\_email|String|邮箱|是|
|7|new\_money|BigDecimal|余额|是|
|8|yonghu\_delete|Integer|假删|是|
|9|create\_time|Date|创建时间|是|
表4.11预约书籍表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|yuyueshuji\_name|String|书籍名称|是|
|3|yuyueshuji\_zuozhe|String|书籍作者|是|
|4|yuyueshuji\_chubanshe|String|出版社|是|
|5|shujigoumai\_types|Integer|书籍类型|是|
|6|yonghu\_id|Integer|用户|是|
|7|yuyueshuji\_time|Date|预约时间|是|
|8|create\_time|Date|创建时间|是|
表4.12用户表表

|序号|列名|数据类型|说明|允许空|
| :-: | :-: | :-: | :-: | :-: |
|1|Id|Int|id|否|
|2|username|String|用户名|是|
|3|password|String|密码|是|
|4|role|String|角色|是|
|5|addtime|Date|新增时间|是|

### 5.1用户信息管理
如图5.1显示的就是用户信息管理页面，此页面提供给管理员的功能有：用户信息的查询管理，可以删除用户信息、修改用户信息、新增用户信息，

还进行了对用户名称的模糊查询的条件

![](/md/blog.018.png)

![](/md/blog.019.png)

图5.1 用户信息管理页面
### 5.2 购买书籍管理
如图5.2显示的就是购买书籍管理页面，此页面提供给管理员的功能有：查看已发布的购买书籍数据，修改购买书籍，购买书籍作废，即可删除，还进行了对购买书籍名称的模糊查询 购买书籍信息的类型查询等等一些条件。

![](/md/blog.020.png)

![](/md/blog.021.png)


图5.2 购买书籍管理页面
### 5.3书籍信息管理
如图5.3显示的就是书籍信息管理页面，此页面提供给管理员的功能有：根据书籍信息进行条件查询，还可以对书籍信息进行新增、修改、查询操作等等。

![](/md/blog.022.png)

![](/md/blog.023.png)

图5.3 书籍信息管理页面
### 5.1书籍借阅管理
如图5.4显示的就是书籍借阅管理页面，此页面提供给管理员的功能有：根据书籍借阅进行新增、修改、查询操作等等。

![](/md/blog.024.png)


图5.4 书籍借阅管理页面

# 










