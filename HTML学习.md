##  **HTML 开始**

**1、HTML 架构**

```java
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"

"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

### 三种：

1.Strict（严格型)

2.Trasitional（过渡型）

3.Frameset（框架型）

***HTML5 基本结构***

<!DOCTYPE html> <html lang="zh-cn">  <head>  <meta charset="utf-8" /> <title>标题</title>  </head> <body>  <p>简明教程</p> </body> </html>

**3、HTML 语言**

- HTML 语言组成

1）标签

> txt 写在尖角号<>里的第一个单词，叫做标记，也叫做标签，也称作元素；

2）属性

> 标记和属性用空格隔开，属性和属性值用等号连接，属性值必须放在双引号内 一个标记可以有多个属性，属性和属性之间用空格隔开，属性不分先后顺序

- HTML 语法

1）常规标记(双标记)：<标记名称 属性 1 名="属性 1 值" 属性 2 名="属性 2 值" ……… >

2）空标记（单标记）：<标记名 属性 1 名="属性 1 值" />

**常用标签**

1）文本标题标签

> 文本标题共有 6 个（h1-h6）
> <h1>一级标题<h1>
> <h2>二级标题<h2>
> ...
> <h6>六级标题<h6>

2）字体倾斜&加粗标记

```java
文本倾斜:

    <i></i>
    <em></em>

文本加粗：
    <b></b>
    <strong></strong>
```

3）下划线

```java
<u></u>
```

4） 换行&水平线

```java
<br>
<hr>
```

5）上标&下标

```java
<sup></sup>
<sub></sub>
```

6）常用转义字符

```java
&nbsp;     不换行空格
&gt;       >右尖括号
&lt;       <左尖括号
&copy;     备案中图标版权
```

7）列表

- 无序列表

```java
<ul>
     <li>列表项内容</li>
     <li>列表项内容</li>
     <li>列表项内容</li>
       ........
</ul>
```

- 有序列表

```java
<ol>
    <li>列表项内容</li>
    <li>列表项内容</li>
    <li>列表项内容</li>
    ........
</ol>
```

> type:规定列表中的列表项目的项目符号的类型
> 语法：<ol type=“ a">
> 1 数字顺序的有序列表（默认值）（1, 2, 3, 4）。
> a 字母顺序的有序列表，小写（a, b, c, d）。
> A 字母顺序的有序列表，大写（A,B,C,D)
> i 罗马数字，小写（i, ii, iii, iv）。
> I 罗马数字，大写（i, ii, iii, iv）。
> start 属性规定有序列表的开始点。(start 的属性值必须是数字)
> 语法：<ol start="5"></ol>

- 自定义列表

```java
<dl>
     dt></dt>
     <dd></dd>
</dl>
```

8）超链接

```java
<a></a>
    属性：
        href = 'url'
        target = "_blank  /  _self";
        title = '文本提示'
    拓展：
        rel = 'nofollow';
```

9） 图片

```java
<img>

    属性：
        src = 'url';
        alt = ' 标签 实例 带有指定替代文本的图像'
        title = '文本提示'
        width = ''
        height = ''
        border = ''
```

**图片 title 和 alt 区别：**

> alt:
> 1、alt属性是考虑到不支持图像显示或者图像显示被关闭的浏览器的用户，以及视觉障碍的用户和使用屏幕阅读器的用户。当图片不显示的时候，图片的替换文字。
> 2、alt属性值的长度必须少于100个英文字符
> 3、alt属性是img标签的必须属性，如果没有特别意义的图片，可以写alt=""
> 4、alt属性是搜索引擎判断图片与文字是否相关的重要依据，alt属性添加到img主要的目的才是为了SEO
> title:
> 1、title属性并不是必须的。
> 2、title属性规定元素的额外信息，有视觉效果，当鼠标放到文字或是图片上时有文字显示。
> 3、title属性并不作为搜索引擎抓取图片的参考，更多倾向于用户体验的考虑。

10）相对路径

- （同级） )当当前文件与目标文件在同一目录下，直接书写目标文件的文件名+扩展名；（上级找下级）
- 当当前文件与目标文件所处的文件夹在同一目录下，写法如下：文件夹名/目标文件全称+扩展名；（下级找上级）
- 当当前文件所处的文件夹和目标文件在同一目录下，写法如下：../目标文件文件名+扩展名；

11）DIV

12）HTML 注释

```java
<!-- 注释 -->
```

## **表格**

**1 、 表格基本结构**

```java
<table>

    <tr>
        <td></td>
        <td></td>
    </tr>

</table>

<!--
    table 为表格
    tr 行
    td 列（每一个单元格）
-->
```

**2、表格的 html 属性**

1）width="表格的宽度"

2）height="表格的高度"

3）border="表格的边框"

4）bordercolor="边框色"

5）cellspacing="单元格与单元格之间的间距"

6）cellpadding=“单元格与内容之间的距离"

7）align="表格水平对齐方式"

取值：left、right、center、valign=“垂直对齐” top\bottom\middle

8）合并单元格属性：(td)

合并列：colspan=“所要合并的单元格的列数"

合并行：rowspan=“所要合并单元格的行数”

**3 、数据行分组**

```java
<thead></thead>
<tbody></tbody>
<tfoot></tfoot>
```

**4 、数据列分组**

```java
<colgroup span="value"></colgroup>
<!--span属性为把几列分为一组-->
```

**5 、列标题**

```java
<th></th>
```

**6、 表格标题**

```java
<caption></caption>
```

**7、表格属性**

> 1、单元格间距：border-spacing:value;说明：单元格间距(该属性必须给 table 添加) 表示单元格边框之间的距离， 不可取负值
> 2、合并相邻单元格边框：border-collapse:separate/collapse;说明：合并相邻单元格边框 (该属性必须给 table 添加) separate(边框分开)默认值；collapse(边框合并)
> 3、无内容时单元格的设置：empty-cells:show/hide;说明：定义当单元格无内容时，是否显示该单元格的边框区域；show：显示 ；hide：隐藏；
> 4、显示单元格行和列的算法(加快运行的速度)：table-layout:auto/fixed;