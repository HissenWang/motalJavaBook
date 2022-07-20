# **开发工具IDEA的介绍、安装、配置优化与快捷键**

# 一、**编码神器-IDEA**

## （一）**IDEA介绍[了解即可，多用在吹牛]**

1、官网下载：

http://www.jetbrains.com/idea/download  

2、官网教程:

 https://www.jetbrains.com/help/idea/install-and-set-up-product.html

3、百度百科介绍：

 [IntelliJ IDEA_百度百科 (baidu.com)](https://baike.baidu.com/item/IntelliJ IDEA/9548353?fromtitle=idea&fromid=1671803&fr=aladdin) 

 IDEA 全称 IntelliJ IDEA，是[java](https://baike.baidu.com/item/java/85979)[编程语言](https://baike.baidu.com/item/编程语言/9845131)开发的集成环境。IntelliJ在业界被公认为最好的java开发工具，尤其在智能代码助手、代码自动提示、[重构](https://baike.baidu.com/item/重构/2182519)、[JavaEE](https://baike.baidu.com/item/JavaEE/3066623)支持、各类版本工具([git](https://baike.baidu.com/item/git/12647237)、[svn](https://baike.baidu.com/item/svn/3311103)等)、[JUnit](https://baike.baidu.com/item/JUnit/1211849)、[CVS](https://baike.baidu.com/item/CVS/405463)整合、代码分析、 创新的[GUI](https://baike.baidu.com/item/GUI/479966)设计等方面的功能可以说是超常的。IDEA是[JetBrains](https://baike.baidu.com/item/JetBrains/7502758)公司的产品，这家公司[总部](https://baike.baidu.com/item/总部/5289033)位于[捷克共和国](https://baike.baidu.com/item/捷克共和国/418555)的首都[布拉格](https://baike.baidu.com/item/布拉格/632)，开发人员以严谨著称的[东欧](https://baike.baidu.com/item/东欧/7149362)[程序员](https://baike.baidu.com/item/程序员/62748)为主。它的[旗舰](https://baike.baidu.com/item/旗舰/4724820)版本还支持[HTML](https://baike.baidu.com/item/HTML/97049)，[CSS](https://baike.baidu.com/item/CSS/5457)，[PHP](https://baike.baidu.com/item/PHP/9337)，[MySQL](https://baike.baidu.com/item/MySQL/471251)，[Python](https://baike.baidu.com/item/Python/407313)等。免费版只支持Java,[Kotlin](https://baike.baidu.com/item/Kotlin/1133714)等少数语言。 公司旗下还有其它产品，比如：

-  WebStorm：用于开发 JavaScript、HTML5、CSS3 等前端技术；

-  PyCharm：用于开发 python

-  CLion：用于开发 C/C++

-  DataGrip：用于开发数据库和 SQL

-  GoLand：用于开发 Go

-  Android Studio：用于开发 android

4、 IntelliJ IDEA 对硬件的要求：

2G 内存的计算机只适合写小程序、小项目或是开发静态页面。Java Web 项目最好的方案是 8G 内存或是以上，硬盘能再用上固态是最好的，因为IntelliJ IDEA 有大量的缓存、索引文件，把 IntelliJ IDEA 的缓存、索引文件放在固态上，IntelliJ IDEA 流畅度也会加快很多。

## （二）**下载-安装[掌握，第一个纸老虎]**

### 1．**下载**

https://www.jetbrains.com/idea/download

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps116.jpg) 

 

### 2．**安装**

#### （1）**点击安装**

本教程所对应的版本2017.3.2版本，其实版本不同，按钮图标和描述一般不会变，所以不必刻意追求最新版本。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps117.jpg) 

**注意:所有软件安装路径中不能出现空格和中文！！！**   

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps118.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps119.jpg) 

第一项，在桌面上创建一个快捷图标，建议勾选上，方便我们在安装后定位 IntelliJ IDEA 安装目录。第二项关联 Java 和 Groovy 文件，建议都不要勾选。因为正常我们会在 Windows 的文件系统上打开这类文件都是为了快速查阅文件里面的内容，如果用 IntelliJ IDEA 关联上之后，便会默认用IntelliJ IDEA 打开，速度缓慢，浪费时间。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps120.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps121.jpg) 

#### （2）**运行并破解**

​	可根据个人需要百度idea服务器破解，或者idea破解码

#### （3）**选择UI主题**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps122.jpg) 

#### （4）**选择插件(跳过)**

这里可以按默认设置，点击下一步，后续可以在settings中修改

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps123.jpg) 

### 3．**目录介绍**

#### （1）**安装目录**介绍

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps124.jpg) 

1. bin：容器，执行文件和启动参数等

2. help：快捷键文档和其他帮助文档

3. jre64：64 位java 运行环境

4. lib：idea 依赖的类库

5. license：各个插件许可

6. plugins：插件
7. redist：注册相关文件

**其中，bin 目录下：**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps125.jpg) 

1. idea.exe 文件是 IntelliJ IDEA 32 位的可行执行文件，IntelliJ IDEA 安装完默认发送到桌面的也就是这个执行文件的快捷方式。

2. idea.exe.vmoptions 文件是 IntelliJ IDEA 32 位的可执行文件的 VM 配置文件

3. idea64.exe 文件是 IntelliJ IDEA 64 位的可行执行文件，要求必须电脑上装有 JDK 64 位版本。64 位的系统也是建议使用该文件。

4. idea64.exe.vmoptions 文件是 IntelliJ IDEA 64 位的可执行文件的 VM 配置文件

5. idea.properties 文件是 IntelliJ IDEA 的一些属性配置文件




VM配置文件修改的原则主要是根据自己机器的内存情况来判断的，个人是建议 8G 以下的机子或是静态页面开发者都是无需修改的。如果你是开发大型项目、Java 项目或是 Android 项目，并且内存大于 8G，建议进行修改：

1. -Xms128m，16 G 内存的机器可尝试设置为 -Xms512m	(设置初始的内存数，增加该值可以提高 Java 程序的启动速度。)
2. -Xmx750m，16 G 内存的机器可尝试设置为 -Xmx1500m	(设置最大内存数，提高该值，可以减少内存 Garage 收集的频率，提高程序性能)

3. -XX:ReservedCodeCacheSize=240m，16G 内存的机器可尝试设置为-XX:ReservedCodeCacheSize=500m	(缓存大小)

#### （2）**配置目录**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps126.jpg) 

1. 对于这个设置目录有一个特性，就是你删除掉整个目录之后，重新启动 IntelliJ IDEA 会再自动帮你再生成一个全新的默认配置，所以很多时候如果你把 IntelliJ IDEA 配置改坏了，没关系，删掉该目录，一切都会还原到默认。

2.  config 目录是 IntelliJ IDEA 个性化化配置目录，或者说是整个 IDE 设置目录。也是我个人认为最重要的目录，没有之一，安装新版本的 IntelliJ IDEA 会自动扫描硬盘上的旧配置目录，指的就是该目录。这个目录主要记录了：IDE 主要配置功能、自定义的代码模板、自定义的文件模板、自定义的快捷键、Project 的 tasks 记录等等个性化的设置。

3. system 目录是 IntelliJ IDEA 系统文件目录，是 IntelliJ IDEA 与开发项目一个桥梁目录，里面主要有：缓存、索引、容器文件输出等等，虽然不是最重要目录，但是也是最不可或缺目录之一。

   

配置文件的位置可以通过修改安装目录bin/idea.properties文件来指定

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps127.jpg) 

上图是 IntelliJ IDEA 一些属性配置，没有 32 位和 64 位之分，修改原则主要根据个人对 IntelliJ IDEA 的个性化配置情况来分析。常修改的就是下面 4 个参数：

1. idea.config.path=${user.home}/.IntelliJIdea/config ，该属性主要用于指向 IntelliJ IDEA 的个性化。配置目录，默认是被注释，打开注释之后才算启用该属性，这里需要特别注意的是斜杠方向，这里用的是正斜杠。

2. idea.system.path=${user.home}/.IntelliJIdea/system ，该属性主要用于指向 IntelliJ IDEA 的系统文件目录，默认是被注释，打开注释之后才算启用该属性，如果你的项目很多，则该目录会很大，如果你的 C 盘空间不够的时候，还是建议把该目录转移到其他盘符下。
3. idea.max.intellisense.filesize=2500，该属性主要用于提高在编辑大文件时候的代码帮助，IntelliJ IDEA 在编辑大文件的时候还是很容易卡顿的。
4. idea.cycle.buffer.size=1024，该属性主要用于控制控制台输出缓存。如果遇到项目开启很多输出的话，那么控制台很快就被刷满了，没办法再自动输出后面内容，这种项目建议增大该值或是直接禁用掉，禁用语idea.cycle.buffer.size=disabled。

## （三）**入门案例[掌握，经典helloworld要来了]**

### 1．**创建普通Java工程**

#### （1）**创建工程并编写代码**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps128.jpg) 

1. Create New Project 创建一个新项目。

2. Import Project 导入一个已有项目。

3. Open 打开一个已有项目。

4. Check out from Version Control 可以通过服务器上的项目地址 Checkout Github 上面项目或是其他 Git 托管服务器上的项目。


![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps129.jpg) 

点击next

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps130.jpg) 

指定名称和位置

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps131.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps132.jpg) 

 显示工具

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps133.jpg) 

界面说明

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps134.jpg) 

1.  工程下的src 目录，用于存放代码。

2.  工程下的.idea 和 .iml 文件都是 IDEA 工程特有的。

3.  .idea 即为 Project 的配置文件目录。

4.  .iml 即为 Module 的配置文件。


设置项目jdk环境

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps135.jpg) 

创建类

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps136.jpg)![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps137.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps138.jpg) 

编写代码

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps139.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps140.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps141.jpg) 

**说明：在 IDEA 里写完代码，不用点击保存。**

运行代码

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps142.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps143.jpg) 

## **（四）常见设置[应用，让IDEA变舒适的关键之一]**

### 1．**显示工具栏图标**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps177.jpg) 

### 2．**查看项目配置(项目源目录、输出以及所依赖的jar****)

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps178.jpg) 

或者

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps179.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps180.jpg) 

 **project language level编译级别是用来告诉IDEA，应该用哪种级别的语法检查项目来提示编码或错误，所以级别一般不能高于jdk版本，否则容易引起误报。**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps181.jpg) 

### 3．**全局默认设置（配置针对整个Idea生效）**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps182.jpg) 

或者

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps183.jpg) 

### 4．**普通设置（针对Project级别，工作空间级别）**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps184.jpg) 

说明

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps185.jpg) 

注意：通过settings进行的普通设置有一些可以全局生效

### 5．**更改字体大小通过ctrl+鼠标滚轮**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps186.jpg) 

### 6．**代码提示不区分大小写**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps187.jpg) 

### 7．**修改主题**

l 修改主题

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps188.jpg) 

### 8．**修改字体**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps189.jpg) 

修改控制台输出字体

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps190.jpg) 

### 9．**修改控制台字体颜色**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps191.jpg) 

### 10．**修改注释的字体颜色(了解)**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps192.jpg) 

1.  Doc Comment – Text：修改文档注释的字体颜色

2.  Block comment(块注释)：修改多行注释的字体颜色

3.  Line comment：修改当行注释的字体颜色


### 11．**设置文件编码（重要）**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps193.jpg) 

说明：

1. Transparent native-to-ascii conversion 主要用于转换 ASCII码表，一般都要勾选，不然 Properties 文件中的注释显示的都不会是中文。
2. BOM for UTF-8 是让编码带bom签名，告诉编辑器当前文件采取何种编码（UTF-16？UTF-32？），会产生更多输出，所以一般不选，选择后会编译报错。

### 12．**设置鼠标悬浮提示**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps194.jpg) 

### 13．**自动导包&优化导包**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps195.jpg) 

### 14．**设置自动编译**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps196.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps197.jpg) 

### 15．**在Editor进行空格与tab缩进设置**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps198.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps199.jpg) 

### 16．**显示行号和方法分割线**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps200.jpg) 

### 17．**去除单词拼写检查**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps201.jpg) 

### 18．**清理缓存和索引**

随着项目越来越大，新编写的代码没有立即生效（引用等），此时可以清理缓存和索引

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps202.jpg) 

通过上面方式清除缓存、索引本质也就是去删除 C 盘下的 system 目录下的对应的文件而已，所以如果你不用上述方法也可以删除整个 system 。当 IntelliJ IDEA 再次启动项目的时候会重新创建新的 system 目录以及对应项目缓存和索引。如果你遇到了因为索引、缓存坏了以至于项目打不开，那也建议你可以直接删除 system 目录，一般这样都可以很好地解决你的问题。

### 19．**设置目录折叠**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps203.jpg) 

### 20．**定位到当前文件所在目录**![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps204.jpg)

### 21．**配置文件的生成模板**

 ```java
/**
 * @author ${USER}
 * @date ${DATE} ${TIME}
 * @description 
 */
 ```

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps205.jpg) 

### 22．**Debug**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps206.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps207.jpg) 

### 23．**省电模式**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps208.png)	如上图标注 1 所示，IntelliJ IDEA 有一种叫做 省电模式 的状态，开启这种模式之后 IntelliJ IDEA 会关掉代码检查和代码提示等功能。所以一般我也会认为这是一种 阅读模式。如果你在开发过程中遇到突然代码文件不能进行检查和提示可以来看看这里是否有开启该功能。 

### 24．**显示内存占用**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps209.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps210.jpg) 

### 25．**设置水平或者垂直分屏编辑**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps211.jpg) 

 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps212.jpg) 

### 26．**设置启动idea或打开项目时提示**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps213.jpg) 

### 27．**设置代码环绕**

Ctrl + Alt + T 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps214.jpg) 

### 28．**取消更新**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps215.jpg) 

### 29．**查看本地文件编辑历史**

类似ctrl+z功能的升级

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps216.jpg) 

### 30．**生成 javadoc**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps217.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps218.jpg) 

zh_CN

-encoding UTF-8 -charset UTF-8

注意，如果项目要求的JDK与实际环境安装的JDK不匹配，可能会导致导出失败，需要调整JDK版本一致。

### 31．**自定义代码模版**

关于模板(Templates)

代码模板的原理就是配置一些常用代码字母缩写，在输入简写时可以出现你预定义的固定模式的代码，使得开发效率大大提高，同时也可以增加个性化。

最简单的例子就是在 Java 中输入 sout 会出现 System.out.println();

Idea中代码模板有两类Live Templates和Postfix Completion

二者的区别：Live Templates 可以自定义，而 Postfix Completion 不可以。同时，有些操作二者都提供了模板，Postfix Templates 较 Live Templates 能快 0.01 秒

官方介绍 Live Templates：

<https://www.jetbrains.com/help/idea/using-live-templates.html>

Postfix Completion

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps219.jpg) 

Live Templates

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps220.jpg) 

1. tli遍历集合/itar遍历数组（使用较多）

2. psvm :  可生成 main  方法 

3. sout : System.out.println()  快捷输出

4. soutp=System.out.println("方法形参名 = " + 形参名);

5. soutv=System.out.println("变量名 = " + 变量);

6. soutm=System.out.println("当前类名.当前方法");

7. “abc”.sout => System.out.println("abc");

8. fori :  可生成 for  循环

9. iter：可生成增强 for 循环

10. itar：可生成普通 for 循环

11. list.for :  可生成集合 list 的 的 for  循环

12. List<String> list = new ArrayList<String>();

13. 输入: list.for 即可输出for(String s:list){}

14. list.fori 或 list.forr

15. ifn ：可生成 if(xxx = null)

16. inn：可生成 if(xxx != null) 或 xxx.nn 或 xxx.null

17. prsf ：可生成 private static final

18. psf：可生成 public static final

19. psfi：可生成 public static final int

20. psfs：可生成 public static final String


 两种模板的区别：有些操作二者都提供了模板，Postfix Templates 较 Live Templates 能快 0.01 秒

经常使用的如下：

 ![1576482299207](https://cdn.jsdelivr.net/gh/HissenWang/images/img/1576482299207.png)

修改现有模板 修改现有模板:Live Templates

如果对于现有的模板，感觉不习惯、不适应的，可以修改：

修改 1 ：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps222.jpg) 



修改 2 ：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps223.jpg) 

类似的还可以修改 psfs。

IDEA 提供了很多现成的 Templates。但你也可以根据自己的需要创建新的Template。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps224.jpg) 

先定义一个模板的组：

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps225.jpg) 

选中自定义的模板组，点击”+”来定义模板。

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps226.jpg) 

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps227.jpg) 

```java
@Test
public void test$VAR1$(){
       $END$ 
}
```

1. Abbreviatio：模板的缩略名称

2. Description：模板的描述

3. Template text：模板的代码片段

4. 应用范围：比如点击 Define，然后在 java 类文件中应用即可

 

##  （五）**IDEA快捷键[应用，让IDEA变舒适的关键之二]**

### 1．**Idea原生快捷键**

| **快捷键**            | **介绍**                                                     |
| --------------------- | ------------------------------------------------------------ |
| Alt + Enter           | 根据光标处所在的问题，提供快速修复选择，光标放在的位置不同提示的结果也不同（万能修复快捷键，同时可以帮助我们生成本地变量==eclipse中的ctrl+1）注意：非个人编码问题导致的错误，都可以尝试使用该快捷键修复 |
| Alt + Insert          | 代码自动生成，如生成对象的 set / get 方法，构造函数，toString() 等 |
| Shift + Shift         | 查找所有文件                                                 |
| Ctrl + D              | 复制当前行到下一行                                           |
| Ctrl + Y              | 删除当前行                                                   |
| Alt + 左方向键        | 向左切换tab                                                  |
| Alt + 右方向键        | 向右切换tab                                                  |
| Ctrl + Alt + 左方向键 | 快速返回上次查看代码的位置（Back）                           |
| Ctrl + Alt + 右方向键 | 快速返回上次查看代码的位置（Forward）                        |
| Ctrl + F              | 在当前文件进行文本查找                                       |
| Ctrl + Shift + F      | 在当前项目进行文本查找                                       |
| Ctrl + R              | 在当前文件进行文本替换                                       |
| Ctrl + Shift + R      | 在当前项目进行文本替换                                       |
| Ctrl + /              | 注释光标所在行代码，会根据当前不同文件类型使用不同的注释符号 |
| Ctrl + Shift + /      | 代码块注释                                                   |
| Ctrl + Alt + L        | 格式化代码，可以对当前文件和整个包目录使用                   |
| Alt + 7               | 显示当前类中的所有方法、全局常量，方法还包括形参和返回值     |
| Alt + F7              | 可以查看一个Java类、方法或变量的直接使用情况。               |
| ctrl + alt +b         | 查看接口的实现类                                             |
| ctrl + h              | 查看类或接口的继承关系                                       |
| F7                    | 在 Debug 模式下，进入下一步，如果当前行断点是一个方法，则进入当前方法体内，Step Into |
| F8                    | 在 Debug 模式下，进入下一步，如果当前行断点是一个方法，则不进入当前方法体内，Step Over |
| F9                    | 在 Debug 模式下，恢复程序运行，但是如果该断点下面代码还有断点则停在下一个断点上，Resume |

### 2．**设置eclipse风格快捷键**

![img](https://cdn.jsdelivr.net/gh/HissenWang/images/img/wps228.jpg) 

 

常用快捷键：

| 提示补全                                     | Alt + /                  |
| -------------------------------------------- | ------------------------ |
| 单行注释                                     | ctrl + /                 |
| 多行注释                                     | ctrl + shift + /         |
| 向下复制一行                                 | Ctrl + alt + down        |
| 删除一行或选中行                             | Ctrl + d                 |
| 向下移动行                                   | Alt + down               |
| 向上移动行                                   | Alt + up                 |
| 万能纠错/生成返回值变量                      | Alt + enter（依然可用）  |
| 退回到前一个编辑的页面 (back)                | Alt + left               |
| 进入到下一个编辑的页面(针对于上条) (forward) | Alt + right              |
| 查看继承关系(type hierarchy)                 | F4                       |
| 格式化代码                                   | ctrl+shift+F             |
| 选中数行，整体往后移动                       | tab                      |
| 选中数行，整体往前移动                       | shift + tab              |
| 查看类的结构：类似于eclipse 的outline        | ctrl+o                   |
| 修改变量名与方法名                           | Alt + shift + r          |
| 大写转小写/ 小写转大写                       | Ctrl + shift + y/x       |
| 生成构造器/get/set/toString                  | Alt + insert（依然可用） |
| Shift+shift                                  | 万能搜索（依然可用）     |
| 查找/替换(当前)                              | Ctrl + f                 |
| 查找(全局)                                   | Ctrl + h                 |
| 查看类的继承结构图                           | Ctrl + ALT+ u            |
| 打开最近改的文件                             | Ctrl + E                 |
| 查找方法在哪里被调用                         | Ctrl + G                 |

 

