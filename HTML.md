[TOC]



***



# 课程介绍

## 1、软件分类

**系统软件**

windows

Linux

macOS

**应用软件**

office等

**游戏软件**

## 2、客户端与服务器

通常情况下，现在的软件一般由了两个部分组成

> **客户端**

用户通过客户端来使用软件

> **服务器**

服务器负责在远程处理业务逻辑

## 3、客户端分类

### 文字客户端

- 古老的方式，通过命令来使用软件

### 图形客户端

- 通过点击拖动等来使用软件。

### 网页

- 通过访问网页来使用软件。所有的网站都属于这个范畴（B/S架构）

## 4、网页的特点

### 优点

- 不需要安装

- 无需更新

- **跨平台**

### 使用的语言

- HTML、CSS、JavaScript

## 5、历史

- ********蒂姆·伯纳斯-李********爵士万维网的发明人

- 1991年8月6日，世界上第一个服务器和第一个网站在**欧洲核子研究中心上线**。

## 6、浏览器和网页

- 浏览器负责将网页渲染成想要的样子

## 7、W3C的建立

- 伯纳斯李1994年建立了**万维网联盟（W3C）**。
- W3C的出现制定了**网页的开发标准**。
- 编写的网页都需要遵循W3C的规范。

## 8、网页的结构

- 根据W3C的标准，一个网页主要有三个部分组成：**结构、表现和行为**

![image-20221227201911036](C:\Users\95806\AppData\Roaming\Typora\typora-user-images\image-20221227201911036.png)

### 结构

- ==HTML 用于描述页面的结构==

### 表现

- ==CSS 用于控制页面中元素的样式==，页面的样式，美化页面

### 行为

- ==JavaScript 用于响应用户操作==，页面的行为

***

# HTML简介

## 网页

### 什么是网页

+ 网站是网页的集合。
+ 网页是网站的一页，通常是HTML格式的文件。
+ 常见的网页后缀名为.html或.htm，统称为HTML文件。

### 什么是HTML

- HTML（Hypertext Markup Lauguage）**超文本标记语言**，它是用来描述网页的一种语言。

- 是一种标记语言。

- HTML 使用**标签**的形式来表示网页中的不同组成部分

- 所谓超文本指的是**超链接**，使用超链接可以让我们从一个页面跳到另一个页面。

- 基本结构

  ```html
  <html> 
      <head>    
      元数据，给浏览器搜索引擎看的 
      </head> 
      <body> 
          想要被看到的内容 
      </body>
  </html>
  ```

### 网页的形成

+ 网页是由网页元素组成，这些元素利用html标签描述出来，然后通过浏览器解析来显示给用户。
+ 是图片、链接、文字、声音等元素组成。

## 常用浏览器

### 常用的浏览器

+ IE、火狐、谷歌、Safari、Opera称为五大浏览器

### 浏览器内核

+ 负责读取网页的内容，整理讯息。计算网页的显示方式并显示页面。

## web标准

+ web标准是由W3C组织和其他组织共同制定的标准的集合。

+ Web标准构成

  ![image-20230402200023107](C:\Users\95806\AppData\Roaming\Typora\typora-user-images\image-20230402200023107.png)

***

# HTML标签

## HTML语法规范

### 基本语法概述

+ HTML标签是由尖括号包围的关键词，例如<html>
+ HTML标签通常是成对出现，第一个是开始标签，第二个是结束标签
+ 有些是单标签

### 标签的关系

> ==包含关系和并列关系==

+ 包含关系（父子关系）

  ```html
  <html> 
      <head>    
      </head> 
  </html>并列关系
  ```

+ 并列关系（兄弟关系）

  ```html
      <head>     
      </head> 
      <body> 
      </body>
  ```

## HTML基本结构标签

### 第一个网页

+ 每一个网页都有一个基本的结构标签（骨架标签），HTML页面也称为HTML文档

例：第一个页面

```html
<html> 
    <head>    
        <title>这是第一个网页</title>
    </head> 
    <body> 
        想要被看到的内容 
    </body>
</html>
```

| 标签名          | 定义       | 说明                                                   |
| :-------------- | :--------- | :----------------------------------------------------- |
| <html> </html>  | HTML标签   | 页面中最大的标签，称为根标签                           |
| <head></head>   | 文档的头部 | head标签中必须设置的标签                               |
| <title></title> | 文档的标题 | 让网页拥有一个属于自己的网页标题                       |
| <body> </body>  | 文档的主体 | 元素包括文档的所有内容，页面的内容，基本都放在body里面 |

## 网页开发工具

### VSCode的使用

+ 生成页面骨架的结构

  **输入！按下Tab键**

### 文档类型的声明标签

 <!DOCTYPE>  文档类型声明，作用是告诉浏览器使用哪一种HTML版本来显示网页

```html
 <!DOCTYPE html> 
```

这句是指HTML5显示网页

+ 注意：

​    ==声明位于文档的最前面。==

### lang语言种类

用来定义当前文本的显示语言

+ en定义语言为英文
+ zh-CN定义语言为中文
+ 注意：en可以显示中文

### 字符集

+ 既便于计算机识别和存储各种文字
+ 在< head>标签中，可以通过< meta>标签的charset属性来规定HTML文档应该用哪一种字符编码

## HTML常用标签

### 标签语义

+ **就是标签的含义**

### 标题标签< h1 >< h6>

+ 为了使网页更具语义化，HTML提供了6个等级的网页标签，即< h1>到< h6>。

+ 单词head的缩写，意为头部，标题

+ 特点

  > 加了标题的文字会变得加粗，字号也会依次变大。

  > 一个标题独占一行

例：

```html
<html> 

    <head>    
        <title>网页</title>
    </head> 

​    <body> 

        <h1>标题标签 </h1>
        <h2>标题标签 </h2>
        <h3>标题标签 </h3>

​    </body>
</html>
```

### 段落和换行标签

#### 段落标签< p>

+ 在网页中，把文字有条理的显示出来，需要将这些文字分段显示，在HTML标签中，< p>标签用于定义段落，它可以将整个网页分为若干个段落。

  ```html
  <p>这是一个段落标签</p>
  ```

+ 标签语义：==分段==

+ 特点

  > 文本会根据浏览器大小自动换行；

  > 段落和段落之间有间隙

#### 换行标签 < br/>

+ 这是一个单标签

  ```html
  <br />
  ```

+ 标签语义：==强制换行==

+ 特点

  >只是简单的开始新的一行，跟段落不同

例：

```html
<html> 
    <head>    
        <title>体育网</title>
    </head> 
    <body> 
        <h1>欢迎回家 </h1>
        <p>北京时间4月2日下午，F1澳大利亚大奖赛在墨尔本阿尔伯特公园赛道展开正赛对决，整场正赛事故不断，赛会三次出红旗，勒克莱尔、阿尔本和拉塞尔、马格努森等8名车手在比赛中先后退赛，红牛车手维斯塔潘虽然出发起步不好，但很快完成超越，并在一波三折的比赛中将优势延续到最后，赢得本赛季第二个分站赛冠军。汉密尔顿和阿隆索收获亚军和季军，中国车手周冠宇排名第9，收获两个积分。

        </p>
        <p>在杆位争夺中，红牛车手维斯塔潘以1分16秒732的成绩收获杆位，<br />梅德赛斯双雄拉塞尔和汉密尔顿在第二和第三位发车，周冠宇排名第17。五盏红灯熄灭，正赛拉开大幕，起步后拉塞尔在1号弯就成功超越维斯塔潘，而法拉利车手勒克莱尔出师不利，与阿斯顿马丁车手斯托尔发生碰撞，勒克莱尔的赛车被顶入到砂石区，这位法拉利车手随即走出赛车，他不得不退赛，这也是勒克莱尔本赛季前三站第2次退赛。</p>
    </body>
</html>
```

### 文本格式化标签

+ 在网页中，有时需要粗体、斜体、下划线等效果

+ 标签语言：==突出重要性==

  | 语义     | 标签                         | 说明                       |
  | -------- | ---------------------------- | -------------------------- |
  | **加粗** | <strong></strong>或者<b></b> | 推荐<strong>，语义更加强烈 |
  | **倾斜** | <em></em>或者<i></i>         | 推荐<em>，语义更加强烈     |
  | 下划线   | <ins></ins>或者<u></u>       | 推荐<ins>，语义更加强烈    |
  | 删除线   | <del></del>或者<s></s>       | 推荐<del>，语义更加强烈    |


### div和span标签（布局）

+ < div> 和 < span>是没有语义的，他们是一个盒子，用来装内容
+ 语法：

```html
<div>这是头部</div>
<span>今日</span>
```

+ div是divsion的缩写，==表示分割、分区==。==span是跨度和跨距==。

+ 特点：

  < div>标签用来布局，独占一行（一行只放一个<div>）。大盒子

  <span>标签用来布局，一行可以放多个。小盒子

### 图像标签和路径

#### 图像标签

+ 在HTML中，利用<img>标签用来定义HTML页面中的图像

+ 语法

  ```html
  <img src="图像URL">
  ```

+ 是一个单标签

+ 图像标签的属性

  | 属性   | 属性值   | 说明                               |
  | ------ | -------- | ---------------------------------- |
  | src    | 图片路径 | 必须属性                           |
  | alt    | 文本     | 替换文本。图像不能显示的文字       |
  | title  | 文本     | 提示文本，鼠标放到图像上，显示文字 |
  | width  | 像素     | 设置图像的宽度,等比例缩放          |
  | height | 像素     | 设置图像的高度                     |
  | border | 像素     | 设置图像的边框粗细                 |

+ 例：

  ```html
  <html> 
      <head>    
          <title>图像标签</title>
      </head> 
      <body> 
          <h4>图像标签的使用 </h4>
          <img src="1.jpg">
          <h4>alt 替换文本。图像不能显示的文字 </h4>
          <img src="1.jpg" alt="学习网">
          <h4>title 提示文本，鼠标放到图像上，显示文字 </h4>
          <img src="1.jpg" alt="学习网" title="欢迎查看">    
          <h4>width 设置图像宽度  </h4>
          <img src="1.jpg" alt="学习网" title="欢迎查看" width="500"/>        
          <h4>height 设置图像高度 </h4>
          <img src="1.jpg" alt="学习网" title="欢迎查看"  height="300"/>   
          <h4>border 设置图像的边框 </h4>
          <img src="1.jpg" alt="学习网" title="欢迎查看"  height="300" border="15"/> 
      </body>
  </html>
  ```

+ 注意点：
  1. 图像的多个属性必须放在标签名的后面。
  2. 属性不分顺序，均用空格分开。
  3. 属性采取键值对的格式，属性 = ”属性值“。

#### 路径

+ 目录文件夹：就是普通的文件夹
+ 根目录：打开目录文件夹的第一层就是根目录
+ 路径
  1. 相对路径
     + 以引用文件所在的位置为参考，而建立的目录路径
  2. 绝对路径
     + 是指目录下的绝对路径，文件的全部路径，通常从盘符开始

### 超链接标签

+ <a>标签

+ 语法格式

  ```html
  <a href="跳转目标" target="目标窗口弹出的方式">文本或图像</a>
  ```

+ 属性

  | 属性   | 作用                                                         |
  | ------ | ------------------------------------------------------------ |
  | href   | 用于指定的链接目标的url地址，（必须属性）当为标签应用href属性时，他就具有超链接的功能 |
  | target | 用于指定连接页面的打开方式，_self是默认的值， _blank为zai新窗口中打开方式（替换当前页面） |

+ 链接分类

  1. 外部链接：例如：< a href="http://www.baidu.com">百度</a>
  2. 内部链接：网络之间相互链接，直接链接内部页面名称即可。例如：< a href="index.html">首页</a>
  3. 空链接：# 来代替。例如< a href="#">空链接</a>
  4. 下载链接：地址链接的是压缩包形式。例如< a href="1.zip">下载</a>
  5. 网页元素链接：在网页中的各种元素（文本、图像、表格、音频、视频等）。例如：< a href="http://www.baidu.com"><img scr="1.jpg"/></a>
  6. 锚点链接：点击链接跳转定位到页面的某一个位置。
     + 在链接文本的href属性中，设置属性值为==#名字==的xings，如< a href="#two">第二</a>
     + 找到目标位置标签，里面添加一个id属性=刚才的名字，如< h3 id ="two''>第二生活</h3>

## 实例01：圣诞老人

```HTml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>实例1</title>
</head>
<body>
    <h1>圣诞节的那些事</h1>
    1.<a href="#ab">圣诞节是怎样由来的</a><br />
    2.<a href="#bc">圣诞老人的由来</a><br />
    3.<a href="#ac">圣诞树的由来</a><br />
    <h2><a id="ab">圣诞节是怎样由来的</a></h2>
    <p>圣诞节是基督教世界最大的节日。一般认为12月25日作为圣诞节可能开始于公元336年的罗马教会。
        4世纪初，1月6日是罗马帝国东部各教会纪念耶稣降生和受洗的双重节日，即上帝通过耶稣向世人显示自己。
         这一天又是罗马历书的冬至节，意味着万物复苏的开始。可能由于这个原因，罗马教会才选择这一天作为圣诞节。
         后来，因为各地教会使用的历书不同，具体日期不能统一，于是就把12月24日到第二年的1月6日定为圣诞节节期（Christmas Tide），
         各地教会可以根据当地具体情况在这段节期之内庆祝圣诞节。 在欧美许多国家里，人们非常重视这个节日，把它和新年连在一起，
         而庆祝活动之热闹与隆重大大超过了新年，成为一个全民的节日。
        12月24日平安夜、12月25日圣诞节的主要纪念活动都与耶稣降生的传说有关 。</p>
    <img src="images/2.jpg">
    <h2 id="bc">圣诞老人的由来</h2>
    <p>圣诞节当然少不了<a href="oldman.html" target="_blank">圣诞老人</a>，根据圣经记载，书中并没有提起这一号人物。到底他是如何成为圣诞的主角之一呢？</p>
    <img src="images/1.jpg">
    <p>相传在一千六百多年前，荷兰巴里地方有一个老人，名叫尼古拉斯，他一生最爱帮助贫穷的人家。
        其中有一次他帮助三个贫穷的少女，送她们三袋金子以逃过被卖的不幸。
    到了一八二二年，由荷兰传教士把这位伟大慈善家的故事传到美国，装扮圣诞老人渐渐地流行于世界各国。
    根据调查，以上故事还有下文；当尼古拉斯偷偷把其中一袋金子送给其中一名女子时，他把金子从其中一个窗户扔进去，
    恰好掉进晾在壁炉上的一只长袜中。于是，将礼物放在圣诞袜子的送礼方法便传到至今。</p>
    <p>在平安夜里，孩子总会把一双双色彩缤纷的袜子挂在床头，然后在袜子旁边放杯热牛奶让圣诞老人喝，
    以让劳苦功高的圣诞老人解渴，并送份大礼给自己。</p>
    <h2 id="ac">圣诞树的由来</h2>
    <p>圣诞一直是庆祝圣诞节不可少的装饰物，如果家中没有圣诞树，就大大减少了过节气氛。关于圣诞树的来源有多种不同的传说。</p>
    <p>其中一个是说：大约在十六世纪，圣诞树最先出现在德国，德国人把长青的松柏枝拿到屋中去摆设，将之成为圣诞树。后来，
    由德国人马丁路德把蜡烛放在树林中的枞树枝，然后点燃蜡烛，使它看起来像是引导人们到伯利恒去。而近今日，人们已经
    改用粉色的小灯泡了。</p>
    <p>另一个传说记载。在很久以前，曾有一位农民，在圣诞节那天遇到一个穷苦小孩，他热情地接待了这个儿童。儿童临走时折
        下一根松枝插在地上，松枝立即变成一棵树，上面都挂满礼物，以答谢农民的好意。</p>
    <p>圣诞树真正出现在圣诞节时，首先见于德国，之后又传入欧洲和美国，并以其优美的姿态，成为圣诞节不可缺少的装饰。圣
        诞树的种类繁多，有天然松柏圣诞树、也有人造圣诞树及白色圣诞树。
    每棵圣诞树上都挂满琳琅满目的装饰品，但每棵树的顶端必定有个特大的星星，象征三博士跟随该星而找到耶稣，而且也只有该
    家庭的一家之主可以把这棵希望之星挂上。</p>
    <img src="images/3.jpg">
    <p>更多内容可以<a href="http://www.baidu.com" target="_blank">百度一下</a></p>
</body>
</html>
```



## HTML中的注释和特殊字符

### 注释

+ 以”<!--"开头，以"-->”结束。
+ 快捷键：ctrl + /

### 特殊字符

+ ![image-20230403171810644](C:\Users\95806\AppData\Roaming\Typora\typora-user-images\image-20230403171810644.png)

***

## 表格标签

+ 主要作用

  主要用于==显示、展示数据==，数据展示的清楚

+ 基本语法

  ```html
  <table>
      <tr>
          <th>姓名</th>
          <td>单元格内的文字</td>
          ...      
      </tr>
      ...
  </table>
  
  ```

  1. < table></table>是用于定义表格的标签
  2. <tr></tr>标签用于定义表格的行，必须嵌套在< table></table>标签中
  3. <td></td>用于定义表格的单元格，必须嵌套在<tr></tr>标签中
  4. 字母td指表格数据（table data），即数据单元格的内容
  5. **<th></th>表头标签，加粗居中，位于第一行**

+ 表格的属性

  | 属性名      | 属性值              | 描述                                            |
  | ----------- | ------------------- | ----------------------------------------------- |
  | align       | left、center、right | 规定表格相对于周围元素的对齐方式                |
  | border      | 1或“”               | 规定表格单元格是否拥有边框，默认为'''',表示没有 |
  | cellpadding | 像素值              | 规定单元边沿与其内容之间的空白，默认为2像素     |
  | cellspacing | 像素值              | 规定单元格之间的空白，默认为2像素               |
  | width       | 像数值或者百分比    | 规定表格的宽度                                  |

+ 表格结构标签

  1. <thead></thead>:用于定义表格的头部。<thead>内部必须用于</tr>标签，一般位于第一行。
  2. <tbody></tbody>:用于定义表格的主体，主要用于放数据本体
  3. 以上标签都存放在< table></table>标签之中

+ 合并单元格

  1. 合并单元格方式：<td colspan="2"></td>

     + 跨行合并：rowspan=“合并单元格的个数”

     + 跨列合并：colspan=“合并单元格的个数”

     + 目标单元格：（写合并代码）

       > 跨行：最上侧单元格为目标单元格，写合并代码

       > 跨列：最左侧单元格为目标单元格，写合并代码

## 列表标签

+ 主要作用：==布局==
+ 分类：无序列表、有序列表和自定义列表

### 	==无序列表==

1. **< ul>标签**表示HTML页面中项目的无序列表，一般会用项目的符号呈现列表项，而列表想使用<li>来定义

2. 基本语法格式：

   ```html
   <ul>
       <li>列表项1</li>
       <li>列表项2</li>
       <li>列表项3</li>
       <li>列表项4</li>
       <li>列表项5</li>
   </ul>
   ```

3. 注意：

   >无序列表的各个列表项之间没有顺序级别之分，是并列的。
   >
   >< ul></ul>中只能嵌套<li></li>，直接在< ul></ul>标签中输入其他标签或者文字是不可以的。
   >
   ><li></li>相当于一个容器，可以容纳所有的元素。
   >
   >无序列表会带有自己的样式属性，实际使用，会用CSS来使用。

4. 例

   ![image-20230405204705401](C:\Users\95806\AppData\Roaming\Typora\typora-user-images\image-20230405204705401.png)

### 有序列表

1. **< ol>标签**用于定义有序列表，列表顺序以数字来显示，并且使用<li>标签来定义列表项

2. 基本语法格式

   ```html
   <ol>
       <li>列表项1</li>
       <li>列表项2</li>
       <li>列表项3</li>
   </ol>
   ```

3. 注意

   > < ol></ol>中只能嵌套<li></li>，直接在< ol></ol>标签中输入其他标签或者文字是不可以的。
   >
   > <li></li>相当于一个容器，可以容纳所有的元素。
   >
   > 有序列表会带有自己的样式属性，实际使用，会用CSS来使用。

### ==**自定义列表**==

1. 作用：经常用于对术语或名词进行解释和描述，定义列表的列表向前没有任何项目符号

2. **< dl>标签**用于定义描述列表（或自定义列表），该标签会与**< dt>**(定义项目/名字)和**< dd>**(描述每一个项目/名字)一起使用

3. 基本语法格式：

   ```html
   <dl>
       <dt>名词1</dt>
       <dd>名词1解释1</dd>
       <dd>名词1解释2</dd>
       <dd>名词1解释3</dd>
   </dl>
   ```

4. 注意：

   >< dl></dl>里面只能包含<dt><dd>。
   >
   ><dt>和<dd>个数没有限制。

5. 例

   ![image-20230405204630281](C:\Users\95806\AppData\Roaming\Typora\typora-user-images\image-20230405204630281.png)

## 表单标签

### 使用场景

![image-20230405204939761](C:\Users\95806\AppData\Roaming\Typora\typora-user-images\image-20230405204939761.png)



### 表单的组成

+ 在HTML中，一个完整的表单通常有**表单域、表单控件（也称为表单元素）**和**提示信息**构成

### 表单域

1. **表单域**是一个**包含表单元素的区域**。

2. 主要作用：利用==< form>==标签，来实现用户信息的手机和传递。**< form>会将他范围之内的信息提交给服务器。**

3. 基本语法格式

   ```html
   <form action="url地址",method="提交方式",name="表单域名称">
       各种表单元素控件    
   </form>
   ```

4. 常用属性

   | 属性   | 属性值   | 作用                                               |
   | ------ | -------- | -------------------------------------------------- |
   | action | url地址  | 用于指定接受并处理表单数据的服务器程序的url地址    |
   | method | get/post | 用于设置表单数据的提交方式，其取值为get或post      |
   | name   | 名称     | 用于指定表单的名称，以区分同一个页面中的多个表单域 |

### 表单控件

#### input输入表单元素 

+ **<input>标签**用于收集用户信息
+ 在<input>标签中，包含一个type属性，
+ 基本格式

```html
<input type="属性值" />
```

+ 注意：

  > <input>标签为单标签。
  >
  > type属性设置不同的属性值用来指定不同的控件类型

+ type属性值及其描述

  | 值       | 描述                                                         |
  | :------- | :----------------------------------------------------------- |
  | button   | 定义可点击按钮（多数情况下，用于通过 JavaScript 启动脚本）。 |
  | checkbox | 定义复选框。                                                 |
  | file     | 定义输入字段和 "浏览"按钮，供文件上传。                      |
  | hidden   | 定义隐藏的输入字段。                                         |
  | image    | 定义图像形式的提交按钮。                                     |
  | password | 定义密码字段。该字段中的字符被掩码。                         |
  | radio    | 定义单选按钮。                                               |
  | reset    | 定义重置按钮。重置按钮会清除表单中的所有数据。               |
  | submit   | 定义提交按钮。提交按钮会把表单数据发送到服务器。             |
  | text     | 定义单行的输入字段，用户可在其中输入文本。默认宽度为 20 个字符。 |

  + 例：

    ```HTml
    <form action="xxx.php",method="get",name="表单域名称" >
        用户名：<input type="text"><br>
        密码：<input type="password"><br>
        <!--单选一-->
        性别：男<input type="radio"> 女<input type="radio"><br>
        爱好：吃饭<input type="checkbox"> 睡觉<input type="checkbox"> 打球<input type="checkbox"><br>
        <input type="submit" value="免费注册">
        <input type="reset" value="重新填写">  
        <input type="button" value="获取验证码"> 
        上传头像：<input type="file"> 
    </form>
    ```

  + 注意：

    >button按钮搭配 JavaScript 

+ 其他属性

  | 属性      | 属性值       | 描述                                          |
  | --------- | ------------ | --------------------------------------------- |
  | name      | 由用户自定义 | 定义input元素的名称                           |
  | value     | 由用户自定义 | 规定input元素的值                             |
  | checked   | checked      | 规定input元素首次加载时应当被选中，默认选中的 |
  | maxlength | 正整数       | 规定输入字段中的字符的最大长度                |

  + 例：

    ```html
    <form>
        用户名：<input type="text" name="username" value="请输入用户名" maxlength="9"><br>
        密码：<input type="password"name="pwd" value="请输入密码" maxlength="9"><br>
        性别：男<input type="radio" name="sex" value="男" checked="cheked"> 女<input type="radio" name="sex" value="女"><br>
        爱好：吃饭<input type="checkbox"> 睡觉<input type="checkbox"> 打球<input type="checkbox" checked="cheked"><br>    
    </form>
    ```

  + 注意：

    > name和value是每一个表单元素都有的属性值，只要给后台人员使用。
    >
    > name表单元素名字，要求单选和复选框中的name一样。
    >
    > **checked属性主要针对单选和复选框**，一打开页面，就选中

+ label标签

  1. ==label标签==用于绑定一个表单元素，当点击时，会自动跳转到表单元素

  2. label标签的form属性和相关的id属性相同

  3. 基本语法格式

     ```html
     <label for="sex">男</label>
     <input type="radio" name="sex" id="sex">
     ```

#### select下拉表单元素

+ < select>中至少包含一对<option>

+ 在<option>中定义selected ="selected"时，当前项即为默认选中项

+ 基本语法格式

  ```html
  <select>
      <option>选项</option>
      <option>黑龙江</option>
      <option甘肃</option>
  </select>
  ```

#### textarea文本域元素

+ 通过<textarea>标签可以轻松创建多行文本输入框。

+ **cols="每行中的字符数",rows="显示的行数"**，实际开发用css来调整大小

+ 基本语法格式

  ```html
  <textarea rows="5" cols="10">文本内容</textarea>
  ```

## 实例02：注册页面

```Html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>注册界面</title>
</head>
<body>
    <h3>欢迎来到注册界面</h3>
    <table width="600">
        <tr>
            <td>性别：</td>
            <td>
                <input type="radio" name="sex" id="nan"><label for="nan"> 男</label>
                <input type="radio" name="sex" id="nv"><label for="nv"> 女</label>
            </td>
        </tr>
        <tr>
            <td>生日：</td>
            <td>
                <select>
                    <option>请选择年份</option>
                    <option>2002年</option>
                    <option>2001年</option>
                    <option>2000年</option>
                    <option>1999年</option>
                    <option>1998年</option>
                    <option>1997年</option>
                    <option>1996年</option>
                </select>
                <select>
                    <option>请选择月份</option>
                    <option>1月</option>
                    <option>2月</option>
                    <option>3月</option>
                    <option>4月</option>
                    <option>5月</option>
                    <option>6月</option>
                    <option>7月</option>
                    <option>8月</option>
                    <option>9月</option>
                    <option>10月</option>
                    <option>11月</option>
                    <option>12月</option>
                </select>
                <select>
                    <option>请选择日</option>
                    <option>1</option>
                    <option>2</option>
                    <option>3</option>
                    <option>4</option>
                    <option>5</option>
                    <option>6</option>
                    <option>7</option>
                    <option>8</option>
                    <option>9</option>
                    <option>10</option>
                    <option>11</option>
                    <option>12</option>
                    <option>13</option>
                    <option>14</option>
                    <option>15</option>
                    <option>16</option>
                    <option>17</option>
                    <option>18</option>
                    <option>19</option>
                    <option>20</option>
                    <option>21</option>
                </select>
            </td>
        </tr>
        <tr>
            <td>所在地区：</td>
            <td><input type="text" value="甘肃"></td>
        </tr>
        <tr>
            <td>学历：</td>
            <td><input type="text" value="本科"></td>
        </tr>
        <tr>
            <td>爱好：</td>
            <td>
                <input type="checkbox" name="love"> 篮球
                <input type="checkbox" name="love"> 跑步
                <input type="checkbox" name="love"> 读书
                <input type="checkbox" name="love"> 足球
                <input type="checkbox" name="love" checked="checked"> 都喜欢
            </td>
        </tr>
        <tr>
            <td>自我介绍：</td>
            <td><textarea rows="5" cols="30">简介</textarea></td>
        </tr>
        <tr>
            <td></td>
            <td><input type="submit" value="免费注册"></td>
        </tr>
        <tr>
            <td></td>
            <td><input type="checkbox">我同意注册条款</td>
        </tr>
        <tr>
            <td></td>
            <td><a href="#">我是会员，立即登录</a></td>
        </tr>
        <tr>
            <td></td>
            <td>
                <h4>我承诺</h4>
                <ul>
                    <li>已经年满18岁</li>
                    <li>所填写内容都是真实的</li>
                </ul>

            </td>
        </tr>
    </table> 
</body>
</html>
```





# Bug

## 锚点链接

+ 错误

```
Cannot GET /%E7%BB%BC%E5%90%88%E6%A1%88%E4%BE%8B01/ab
```

+ 解决

锚点链接有误
