# HTML 学习笔记

*该文本用于记载学习html过程中遇到的一些知识点与问题*



## 1. HTML 介绍



### 1.1 什么是HTML

* HTML 的全称为“Hyper Text Markup Language"（超文本标记语言）
* HTML 是创建网页的最基本标记语言
* HTML 用于描述网页的结构`structure`
* HTML 由一系列的元素 `elements` 组成
* HTML 元素告诉浏览器该如何展示内容
* HTML 元素标签描述的内容大致为”这是一个标题“，”这是一段正文“，”这是一个链接“ 等等



### 1.2 一个简单的Html案例

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <h1>
            My First Heading
        </h1>
        <p>
            My first paragraph.
        </p>
    </body>
</html>
```



*案例详解*

* <! DOCTYPE html> 用来宣言定义当前的文件是一个 HTML5 文件
* < html>元素是HTML 页面的根标签
* < head>元素包含了多种关于HTML页面的信息
* < title> 元素为HTML 页面指定了标题信息（会显示在浏览器的标题栏中或者页面栏中）
* < body> 元素定义的该文件的”身体“部分，也是所有可视内容的容器，像是headings,paragraphs,images,hyperlinks,tables,lists 等等
* < h1>元素定义了一个大标题
* < p>元素定义的一个段落



### 1.3 什么是HTML元素

一个 HTML 元素由一个开始标签、内容、结束标签进行定义：

```html
<tagname>Content goes here...</tagname>
```

HTML **元素**是由开始标签到结束标签内包含的任何事物：

```html
<h1>
    My First Heading
</h1>
<br>
<p>
    My first paragraph.
</p>
```

| 开始标签 | 元素内容           | 结束标签 |
| -------- | ------------------ | -------- |
| <h1>     | My First Heading   | </h1>    |
| <p>      | My first paragraph | </p>     |
| <br>     | none               | none     |

> **注意**：一些 html 元素没有内容（像是 `<br>` 标签）。这些元素被称之为空元素。空元素没有结束标签！



### 1.4 页面浏览器

页面浏览器（Chrome、Edge、Firefox、Safari）的目的是用来读取 html 文件并且将他们进行正常展示的。

浏览器将不会展示HTML 标签，而是根据他们决定如何展示文件：

![View in Browser](https://www.w3schools.com/html/img_chrome.png)



### 1.5 HTML 页面结构

以下是HTML页面的可视化结构：



> 注意在 `<body>` 部分内部的内容（如上图白色部分展示的区域）将会被展示在浏览器中。而在`<title>` 元素内部中的内容将会被展示在浏览器的标题栏或者页面的分栏中。



## 2. HTML 基础

*在这一章我们将展示一些基础的HTML范例*



### 2.1 HTML 文件

所有的HTML文件必须以文件类型声明作为开标题：`<!DOCTYPE html>`。

HTML文件本身以 `<html>` 开标题并以 `</html>` 作为结束。

HTML文件中可视的部分在`<body>` 和 `</body>` 之间。



范例如下：

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>
            My First Paragraph.
        </h1>
        <p>
            My first paragraph.
        </p>
    </body>
</html>
```



### 2.2 `<!DOCTYPE html>`声明

`<!DOCTYPE html>` 声明代表一种文件类型，帮助浏览器正确的展示网页。

它必须有且仅能出现一次，并且是在页面的顶上（在任何HTML 标签之前）。

 `<!DOCTYPE>` 对大小写并不敏感。

`<!DOCTYPE>` 声明为HTML5的范例是：

```html
<!DOCTYPE html>
```



### 2.3 HTML 标题

HTML 标题以`<h1>` 到 `<h6>` 标签进行定义。

`<h1>` 定义了最为重要的标题部信息，`<h6>` 定义最不重要的标题部信息。

范例：

```html
<h1>
    This is heading 1
</h1>
<h2>
    This is heading 2
</h2>
<h3>
    This is heading 3
</h3>
```



### 2.4 HTML 段落

HTML 段落以`<p>` 标签进行定义：

范例：

```html
<p>
    This is a paragraph.
</p>
<p>
    This is another paragraph.
</p>
```



### 2.5 HTML 链接

HTML 链接以 `<a>` 标签进行定义。

范例：

```html
<a href="http://www.google.com">This is Google</a>
```

该链接的目的地由 `href` 特性进行指定。

特性用来给 HTML 元素提供额外的信息。



### 2.6 HTML 图像

HTML 图像通过 `<img>` 标签进行定义。

该标签有以下特性：源文件(`src`)，可选文字(`alt`)、宽度`width`以及高度`height` 

> 案例：
>
> ```html
> <img src="taran_dasha.jpg" alt="taran dasha" width="104" height="142">
> ```
>
> 



## 3. HTML 元素

*一个 HTML 元素由开始标签、正文、结束标签组成*



### 3.1 HTML 元素

HTML **元素** 是由开始标签到结束标签内的任何事物

```html
<tagname>Content goes there...</tagname>
```

一些使用 HTML 元素的案例：

```html
<h1>
    My First Heading
</h1>
<br>
<p>
    My first paragraph.
</p>
```

| 开始标签 | 元素内容           | 结束标签 |
| -------- | ------------------ | -------- |
| <h1>     | My First Heading   | </h1>    |
| <p>      | My first paragraph | </p>     |
| <br>     | none               | none     |

> **注意：**一些HTML元素没有任何的正文（像是`<br>` 元素）。这些元素被称之为空元素。空元素没有结束标签。



### 3.2 嵌入HTML 元素

HTML元素可以被嵌入（这意味着元素可以包含其他元素）。

所有的HTML文件都是层层嵌套的HTML元素组成。

以下案例包含了四个HTML 元素（`<html>`，`<body>`,`<h1>`,`<p>`）：

> 案例：
>
> ```html
> <!DOCTYPE hmtl>
> <html>
>  <body>
>      <h1>
>          My First Heading
>      </h1>
>      <p>
>          My first paragraph.
>      </p>
>  </body>
> </html>
> ```
>
> 

**案例解释**

`<html>` 元素是根元素，它定义了整个HTML 文件。

它有一个开始标签`<html>` 以及一个结束标签 `</html>`。

然后，在`<html>` 元素内部有一个`<body>` 元素：

> ```html
> <body>
>  <h1>
>      My First Heading
>  </h1>
>  <p>
>      My first paragraph.
>  </p>
> </body>
> ```

`<body>` 元素定义了文件的身体部分。

它有一个开始标签`<body>` 和一个结束标签`</body>`。

然后，在`<body>`元素内部有与两个其他元素：`<h1>` 和 `<p>`：

> ```html
> <h1>
>  My First Heading
> </h1>
> <p>
>  My first paragraph.
> </p>
> ```

`<h1>` 元素定义了 HTML 的标题部。

它有一个开始标签`<h1>` 以及一个结束标签 `</h1>`

> ```html
> <h1>
>  My First Heading
> </h1>
> ```

`<p>`标签定义了一个段落。

它有一个开始标签`<p>`  和一个结束标签 `</p>`：

> ```html
> <p>
>  My first paragraph.
> </p>
> ```



**注意：永远别忘记结束标签**

哪怕你忘了结束标签，一些 HTML 元素仍然可以正常展示

> 案例：
>
> ```html
> <html>
>  <body>
>      <p>
>          This is a paragraph
>      <p>
>          This is a paragraph
>  </body>
> </html>
> ```
>
> 然而，永远不要依赖以上的写法！如果你忘了加上结束标签都有可能造成一些不可预料的结果和错误！



### 3.3 空HTML元素

不包含任何内容的HTML 元素被称之为空元素。

`<br>` 标签定义了一条分界线，并且该元素没有结束标签。

> 案例：
>
> ```html
> <p>
>  This is a <br> paragraph with a line break.
> </p>
> ```



### 3.4 HTML 对大小写并不敏感

HTML 标签对大小写并不是那么的敏感：`<P>` 与 `<p>` 有着相同的含义

HTML 标准并不要求使用小写的标签，但 W3C **推荐** 在HTML 中使用小写的标签，并且像在XHTML这类更加严格的文件类型中 **要求** 使用小写的标签



### 3.5 HTML 标签参考

https://www.w3schools.com/tags/default.asp

可以在上面这个链接中找到标签对应的描述信息





## 4. HTML 特性

*HTML 特性为HTML 元素提供额外的信息*



### 4.1 HTML 特性

* 所有的HTML元素都能有**特性**
* 特性为HTML元素提供**额外的信息**
* 特性总是在**开始标签**中被定义
* 特性通常以键值对的形式存在像是：**name="value"**



### 4.2 href 特性

`<a>` 标签用于定义一个超链接。`href` 特性指定该链接前往的页面的URL：

> 案例：
>
> ```html
> <a href="http://www.google.com">This is Google</a>
> ```

后面可以学习到更加详细的介绍



### 4.3 src 特性

`<img>` 标签被用来在HTML 页面中嵌入一张图片。`src` 特性指定了被展示的图片的路径：

> 案例：
>
> ```html
> <img src="taran_dasha.jpg">
> ```

有两种方式可以通过 `src` 特性来指定 URL:

1. **绝对URL**：链接指向一个在其他网站进行管理的外部图片。例如：src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.pinterest.com%2Fi0978266602%2Fdasha-taran%2F&psig=AOvVaw2rx_QLFvhK0X1ddB1erRh0&ust=1639917593858000&source=images&cd=vfe&ved=0CAgQjRxqFwoTCJjb_p-v7fQCFQAAAAAdAAAAABAR"

   **注意**：外部图片可能会存在版权问题。如果你没有获得权限去使用它，你可能会违反版权法。另外，你无法控制外部图片。它可能会被突然移除或者更换。

2. **相对URL**：链接指向一个在网站内部进行管理的图片。就像在例子中展示的那样，该URL并没有包含全部的路径名称。如果该URL没有带一个短路径，它将与当前页面进行直接关联。例如：src="img_girl.jpg"。如果URL携带了一个短路径，它将会根据这个路径进行关联。比如说:src="/images/img_girl.jpg"

   **小贴士**：最好是使用相对URL，这样哪怕该改变了前缀域名信息也不会崩掉。



### 4.4 宽度与高度特性

`<img>` 标签也应该包含`width`宽度与`height` 高度特性，这两个特性制定了图片的像素高与像素宽：

> 案例：
>
> ```html
> <img src="img_girl.jpg" width="500" height="600">
> ```



### 4.5 alt 特性

`<img>` 标签中的 `alt` 特性用来给图像指定一个备用文本，如果因为一些原因导致图片无法展示。比方说链接速度过慢、`src`特性指向错误或者如果用户使用的是一个屏幕阅读器。

> 案例：
>
> ```html
> <img src="img_girl.jpg" alt="Girl with a jacket">
> ```

你可以在后续的章节内学到更多。



### 4.6 样式特性

`style` 特性用来给元素添加样式，比如说颜色、字体、大小等等

> 案例：
>
> ```html
> <p style="color:red;">
>  This is a red paragraph.
> </p>
> ```

你可以在后续章节内学到更多



### 4.7 语言特性

你应该总是在`<html>` 标签中包含一个 `lang` 特性，来宣告该网页使用的语言。这将会帮助搜索引擎和浏览器进行搜索与展示。

以下案例展示如何设置英文为网页的语言：

> ```html
> <!DOCTYPE html>
> <html lang="en">
>  <body>
>      ...
>  </body>
> </html>
> ```

在`lang` 特性中可以在语言代码里添加国家代码。因此，最初开始的两个字符定义该HTML页面的语言，后面两个字符定义国家。

以下案例展示如何在页面设置英文为语言、美国为国家：

> ```html
> <!DOCTYPE html>
> <html lang="en-US">
>  <body>
>      ...
>  </body>
> </html>
> ```

https://www.w3schools.com/tags/ref_language_codes.asp

你可以在以上链接中找到所有的语言代码相关参考



### 4.8 标题特性

`title` 特性定义该元素的一些额外信息。

当你的鼠标悬浮在该特性之上的时候，`title` 特性内的值会以“工具指南”的形式展示在页面上

> 范例：
>
> ```html
> <p title="I'm a tooltip">
>  This is a paragraph.
> </p>
> ```



**我们推荐：永远给特性值加上引号**

HTML 标准并没有要求给特性值加上引号。

然而，W3C **建议** 在html中使用引号，并且**要求**在类似于XHTML这类强语法文档中使用引号。

> 好的例子：
>
> ```html
> <a href="http://www.google.com">This is Google</a>
> ```
>
> 坏的例子：
>
> ```html
> <a href=http://www.google.com>This is Google</a>
> ```

有的时候你不得不使用引号。比如下面这个例子将无法正常的展示，因为它包含了一个空格：

> 范例：
>
> ```html
> <p title=About TaranDasha>
>  This will not display
> </p>
> <p title="About TaranDasha">
>  This will display
> </p>
> ```

> 我们建议永远在特性值两侧加上引号



**单引号还是双引号？**

使用双引号来包裹HTML特性是HTML中最常见的方式，但单引号同样可以被使用。

在一些场景中，当特性值本身包含双引号，使用单引号在外部进行包裹也是可行的：

> 范例：
>
> ```html
> <p title='John "Shotgun" Nelson'>
>  Just a little display
> </p>
> ```

反之亦然

> 范例：
>
> ```html
> <p title="John 'Shotgun' Nelson">
>  Just a little display like above.
> </p>
> ```



### 4.9 章节概括

* 所有的HTML 元素都有**特性**
* `<a>` 标签的 `href` 特性指定了链接指向的页面的URL
* `<img>` 标签的 `src` 特性制定了图片展示的路径
* `<img>` 标签的`height` 和 `width` 特性提供了图片的尺寸信息
* `<img>` 标签的 `alt` 特性给图片提供了一个备份信息
* `style` 特性通常用来给元素添加样式，像颜色、字体、大小等等
* `<html>` 标签中的`lang` 特性宣称了该网页使用的语言
* `title` 特性给元素定义了一些额外的信息



### 4.10 HTML 特性参考

https://www.w3schools.com/tags/ref_attributes.asp

上面的链接给出了所有的HTML 特性以及描述



## 5. HTML 标题部

*HTML 标题部主要用来在页面展示标题或副标题*



### 5.1 HTML 标题部

HTML 标题部以`<h1>` 标签到 `<h6>` 标签进行定义。

`<h1>` 定义最重要的标题部信息。`<h6>` 定义最不重要的标题部信息。

> 范例：
>
> ```html
> <h1>
>  Heading 1
> </h1>
> <h2>
>  Heading 2
> </h2>
> <h3>
>  Heading 3
> </h3>
> <h4>
>  Heading 4
> </h4>
> <h5>
>  Heading 5
> </h5>
> <h6>
>  Heading 6
> </h6>
> ```



> **注意**：浏览器会自动给标题部信息前或者后添加一些空格作为余量



### 5.2 标题部信息很重要

搜索引擎以页面的标题部信息作为你的网页的结构以及正文的索引进行查找。

用户通常依靠标题部信息来浏览网页。因此使用标题部信息来展示文档的结构非常重要。

`<h1>`标题应该被用来作为主要标题，然后是`<h2>` ，接着是`<h3>` 等等等等诸如此类。



> **注意**：使用HTML 标题部信息只能用作标题部。不要使用标题部信息来对文本进行**放大**或者**加粗**。



### 5.3 更大的标题部信息

每一个HTML 标题部信息都有一个默认的尺寸。然而，你可以通过`style` 特性为你的任何标题部信息指定尺寸大小，使用 CSS样式中的`font-size` 属性。

> 范例：
>
> ```html
> <h1 style="font-size:60px;">
>  Heading 1
> </h1>
> ```



### 5.4 HTML 标签参考

https://www.w3schools.com/tags/default.asp



## 6. HTML 段落

*一个段落总是会由新的一行开始，并且通常是文本的一部分*



### 6.1 HTML 段落

HTML `<P>` 元素定义一个段落。

段落总是在新的一行开始，而且浏览器会自动在段落前或段落后补上一些空格作为余量。

> 范例：
>
> ```html
> <p>
>  This is a paragraph
> </p>
> <p>
>  This is another paragraph
> </p>
> ```



### 6.2 HTML 展示

你无法得知HTML页面会被怎样展示。

是大屏还是小屏，或者说自定义尺寸的窗口化等等都会造成不同的展示结果。

在HTML中，你无法通过在HTML代码中添加多余的空格与额外的空行改变展示的效果。

浏览器在页面展示的时候会自动将这些多余的空格与空行进行移除。

> 范例：
>
> ```html
> <p>
>  This paragraph
>  contains a lot of lines
>  in source code,
>  but the browser
>  ignores it
> </p>
> <p>
>  This paragraph
>  contains             a lot of spaces
>  in the source           code,
>  but the           browser
>  igonres it.
> </p>
> ```



### 6.3 HTML 水平分隔线

`<hr>`标签在HTML 中定义了一个“专题”隔断，并且通常以水平分隔线的形式存在。

`<hr>` 标签通常被用来在HTML中分隔上下文（或表示正文内部内容的转换）:

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1>This is heading 1</h1>
>      <p>This is a paragraph.</p>
>      <hr>
>      <h2>This is heading 2</h2>
>      <p>This is some another text.</p>
>  </body>
> </html>
> ```

`<hr>` 标签是空标签，意味着他没有结束标签



### 6.4 HTML 分隔行

`<br>` 元素定义一条分隔行。

如果你不想新开一个段落但又需要一个分隔行的时候通常可以使用`<br>`标签。

> 范例
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>This is <br>a paragraph <br> with line breaks.</p>
>  </body>
> </html>
> ```



### 6.5 诗歌问题

下面这首诗会在一行内被展示：

> 范例
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>
>          My Bonnie lies over the ocean.
> 
>          My Bonnie lies over the sea.
> 
>          My Bonnie lies over the ocean.
> 
>          Oh, bring back my Bonnie to me.
>      </p>
>  </body>
> </html>
> ```



### 6.6 解决办法 - HTML `<pre>` 元素

`<pre>` 元素用来定义一个预格式化文本。

`<pre>` 元素内部的文本会被以固定宽度的字体（通常是Courier字体）进行展示，并且保留了全部的空格和空行。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <pre>
>          My Bonnie lies over the ocean.
> 
>          My Bonnie lies over the sea.
> 
>          My Bonnie lies over the ocean.
> 
>          Oh, bring back my Bonnie to me.
>      </pre>
>  </body>
> </html>
> ```



## 7. HTML 样式

*`style` 特性用来给元素添加样式，诸如颜色、字体、大小等等。*



> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>I am normal</p>
>      <p style="color: red;"> I am red</p>
>      <p style="color: blue;">I am blue</p>
>      <p style="font-size: 50px;">I am bigger</p>
>  </body>
> </html>
> ```



### 7.1 HTML 样式属性

设置HTML 元素的样式，可以通过使用 `style` 属性来完成。

HTML `style` 属性有以下语法：

```html
<tagname style="property:value;"></tagname>
```

***property*** 是一个CSS属性，而 ***value*** 是一个CSS值。

> 后续会对CSS进行学习



### 7.2 背景色

CSS `background-color` 属性用于定义元素的背景色

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body style="background-color: powderblue;">
>      <h1>This is a heading</h1>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```



> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="background-color: powderblue;">This is a heading</h1>
>      <p style="background-color: tomato;">This is a paragraph.</p>
>  </body>
> </html>
> ```



### 7.3 文本颜色

CSS `color` 属性用于定义HTML 元素中文本的颜色：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="color: blue;">This is a heading</h1>
>      <p style="color: red;">This is a paragraph</p>
>  </body>
> </html>
> ```



### 7.4 字体

CSS `font-family` 属性用于定义HTML元素中使用的字体：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="font-family: Verdana, Geneva, Tahoma, sans-serif;">This is a heading</h1>
>      <p style="font-family: 'Courier New', Courier, monospace;">This is a paragraph.</p>
>  </body>
> </html>
> ```



### 7.5 字体大小

CSS `font-size` 属性用于定义HTML元素的文本大小

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="font-size: 300%;">This is a heading</h1>
>      <p style="font-size: 160%;">This is a paragraph</p>
>  </body>
> </html>
> ```



### 7.6 文本位置

CSS `text-align` 属性用于定义HTML元素的水平文本位置：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="text-align: center;">Centered heading</h1>
>      <p style="text-align: center;">Centered paragraph</p>
>  </body>
> </html>
> ```



### 7.8 章节总结

* `style` 属性用于指定元素的样式
* `background-color` 属性用于指定元素的背景色
* `color` 属性用于指定文本的颜色
* `font-family` 属性用于指定字体
* `font-size` 属性用于指定字体大小
* `text-align` 属性用于指定文本位置



## 8. HTML 文本格式化

*HTML 包含了许多将文本进行特殊格式化的元素*



> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p><b>This text is bold</b></p>
>      <p><i>This text is italic</i></p>
>      <p>This is <sub>subscript</sub> and <sup>superscript</sup></p>
>  </body>
> </html>
> ```



### 8.1 HTML 格式化元素

格式化元素被用来展示以下几种特殊格式文本：

* `<b>` - 粗体文本
* `<strong>` - 重要的文本
* `<i>` - 斜体文本
* `<em>` - 强调文本
* `<mark>` - 标记文本
* `<small>` - 小文本
* `<del>` - 被删除文本
* `<ins>` - 内嵌文本
* `<sub>` - 下标文本
* `<sup>` - 上标文本



### 8.2 HTML `<b>` 和 `<strong>` 元素

HTML `<b>` 元素定义一个加粗本文且不带任何额外的重要元素。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p><b>This text is bold</b></p>
>  </body>
> </html>
> ```

HTML `<strong>` 元素以强重要性来定义元素。文本内部通常是以粗体进行表示。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p><strong>This text is important</strong></p>
>  </body>
> </html>
> ```



### 8.3 HTML `<i>` 和 `<em>` 元素

HTML `<i>` 元素用来定义一段以备注情绪或者音调阅读的文本。文本内部通常以斜体进行展示。

**贴士**：`<i>` 标签通常用来注明一段学术名词、一段其他语言的句子、一个想法、一艘船的名称等等

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p><i>This text is italic</i></p>
>  </body>
> </html>
> ```

HTML `<em>` 元素定义强调文本。内容通常以斜体进行展示。

**贴士**：一个屏幕阅读器通常都会重读`<em>` 标签内部的文本

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p><em>This text is emphasized</em></p>
>  </body>
> </html>
> ```



### 8.4 HTML `<small>` 元素

HTML `<small>` 用于定义一个小文本：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p><small>This is some smaller text.</small></p>
>  </body>
> </html>
> ```



### 8.5 HTML `<mark>` 元素

HTML `<mark>` 元素定义应该被标记或者高光注明的文本：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>Do not forget to buy <mark>milk</mark> today.</p>
>  </body>
> </html>
> ```



### 8.6 HTML `<del>` 元素

HTML `<del>` 元素用来定义一段已经从文件中被删除的文本。浏览器通常会在被删除的文本上划一条线：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>My favorite color is <del>blue</del> red.</p>
>  </body>
> </html>
> ```



### 8.7 HTML `<ins>` 元素

HTML `<ins>` 元素定义了文件中被插入的文本，浏览器通常会给被插入的文本加一条下划线：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>My favourite color is <del>blue</del> <ins>red</ins>.</p>
>  </body>
> </html>
> ```



### 8.8 HTML `<sub>` 元素

HTML `<sub>` 元素用于定义下标文本。下标文本在表现上只有正常的一半大小，并且有些时候的字体也比正常的要小。下标文本可以被用来表示一些化学公式，比如H2O

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>H<sub>2</sub>O</p>
>  </body>
> </html>
> ```



### 8.9 HTML `<sup>` 元素

HTML `<sup>` 元素定义上标文本。上标文本通常以半个字符的高度进行展示。同上，上标文本可以用来作为脚注，如下：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>WWW<sup>[1]</sup></p>
>  </body>
> </html>
> ```



## 9. HTML 引述和引文元素

*在本章节中我们将会亲身体验`<blockquote>`、`<q>`、`<abbr>`、`<address>`、`<cite>` 和 `<bdo>` HTML 元素*

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>Here is a quote from WWF's website:</p>
>      <blockquote cite="http://www.worldwildlife.org/who/index.html">
>          For 50 years, WWF has been protecting the future of nature.
>          The world's leading conversation organization, WWF works in 100
>          countries and is supported by 1.2 million members in the United
>          States and close to 5 million globally.
>      </blockquote>
>  </body>
> </html>
> ```



### 9.1 HTML `<blockquote>` 引文

HTML `<blockquote>` 元素定义了从其他源处引用的部分。

浏览器通常会对 `<blockquote>` 元素包围的部分进行缩进。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>Here is a quote from WWF's website:</p>
>      <blockquote cite="http://www.worldwildlife.org/who/index.html">
>          For 50 years, WWF has been protecting the future of nature.
>          The world's leading conversation organization, WWF works in 100
>          countries and is supported by 1.2 million members in the United
>          States and close to 5 million globally.
>      </blockquote>
>  </body>
> </html>
> ```



### 9.2 HTML `<q>` 短引用

HTML `<q>` 标签用来定义短引用。

浏览器正常情况下会对引用部分插入引号

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
>  </body>
> </html>
> ```



### 9.3 HTML `<abbr>` 缩写

HTML `<abbr>` 元素用于定义缩写或者首字母缩略语，像是“HTML","Mr"，"Dr","ASAP","ATM"。

标记上缩写可以为浏览器、翻译系统以及搜索引擎提供有效信息。

**贴士**：使用全局标题属性来让你的鼠标悬浮在元素上时展示缩略语的详细描述

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
>  </body>
> </html>
> ```



### 9.4 HTML `<address>` 提供联系信息

HTML `<address>` 标签为文档或者文章的作者/持有者定义联系信息。

联系信息可以是邮箱、URL、物理地址、手机号、社交媒体等等。

`<address>` 中展示的文本通常是以斜体进行渲染，浏览器经常会在`<address>` 元素前或后添加换行。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <address>
>          Written by John Doe. <br>
>          Visit us at: <br>
>          Example.com <br>
>          Box 564, Disneyland <br>
>          USA
>      </address>
>  </body>
> </html>
> ```



### 9.5 HTML `<cite>` 工作标题

HTML `<cite>` 标签用于定义创造性工作的标题（比如一本书、一首诗、一首歌、一部电影、一幅画、一栋建筑等等）。

**注意**：一个人的名字并不是工作的标题。

`<cite>` 元素内部的文本通常以斜体进行渲染。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p><cite>The Scream</cite> by Edward Munch. Painted in 1893.</p>
>  </body>
> </html>
> ```



### 9.6 HTML `<bdo>` 逆向覆写

BDO 的全称是 逆向覆写。

HTML `<bdo>` 标签用来将当前的文本方向进行逆转：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <bdo dir="rtl">This text will be written from right to left.</bdo>
>      <br>
>      <bdo dir="rtl">我自远方而来</bdo>
>  </body>
> </html>
> ```



## 10. HTML `<comment>`

*HTML 注释并不在浏览器中展示，但它们可以帮助你对HTML源码进行记录*



### 10.1 HTML `<comment>` 标签

你可以通过下面这种语法为HTML源码添加注释：

> ```html
> <!-- Write your comments here -->
> ```

注意到在开始标签内有一个感叹号，但结束标签内没有这个感叹号。

> **贴士**：浏览器并不会展示注释内容，但他们可以帮你对源码进行记录。



### 10.2 添加注释

有了注释，你就在你的HTML 代码中放置提示信息和提醒信息：

> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <!-- This is a comment -->
>      <p>This is a paragraph.</p>
>      <!-- Remeber to add more information here -->
>  </body>
> </html>
> ```



### 10.3 隐藏正文

注释可以被用来隐藏正文。

当你想要暂时将内容隐藏起来的时候就可以用这个办法。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html lang="en">
> <head>
>  <meta charset="UTF-8">
>  <meta http-equiv="X-UA-Compatible" content="IE=edge">
>  <meta name="viewport" content="width=device-width, initial-scale=1.0">
>  <title>Document</title>
> </head>
> <body>
>  <p>This is a paragraph.</p>
>  <!-- <p>This is another paragraph</p> -->
>  <p>This is a paragraph too.</p>
> </body>
> </html>
> ```

你也可以隐藏不止一行，任何在 `<!--` 以及 `-->` 之间的内容都会在展示时被隐藏。

> 范例：
>
> 隐藏一片区域的HTML 代码：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>This is a paragraph</p>
>      <!-- <p>Look at this cool image: </p>
>      <img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.reddit.com%2Fr%2FDashaTaran%2Fcomments%2Fga6j7g%2Fpretty_eyes%2F&psig=AOvVaw2BxrmsZaCWH4kQri9TFSZA&ust=1640270684838000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCIiSwc7S9_QCFQAAAAAdAAAAABAI" alt="Taran Dasha"> -->
>      <p>This is a paragraph too.</p>
>  </body>
> </html>
> ```

注释通常也对debug HTML 有所帮助，因为你可以一行行的注释HTML代码来发现问题出在哪里。



### 10.4 隐藏行内正文

注释可以用来隐藏HTML代码中内部的部分

> 范例：
>
> 隐藏一句话中的一部分：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <p>This <!-- great text is --> a paragraph.</p>
>  </body>
> </html>
> ```



## 11. HTML 颜色

*HTML 颜色可以通过预定义的颜色名或者RGB、HEX、HSL、RGBA或者HSLA值等等进行定义*



### 11.1 颜色名称

在HTML中，颜色可以通过颜色的名字进行使用

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="background-color: tomato;">Tomato</h1>
>      <h1 style="background-color: orange;">Oragne</h1>
>      <h1 style="background-color: dodgerblue;">dodgerblue</h1>
>      <h1 style="background-color: mediumseagreen;">mediumseagreen</h1>
>      <h1 style="background-color: gray;">gray</h1>
>      <h1 style="background-color: slateblue;">slateblue</h1>
>      <h1 style="background-color: violet;">violet</h1>
>      <h1 style="background-color: lightgray;">lightgray</h1>
>  </body>
> </html>
> ```



### 11.2 背景色

你可以给HTML元素设置背景色：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="background-color: dodgerblue;">Hello world</h1>
>      <p style="background-color: tomato;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
>  </body>
> </html>
> ```



### 11.3 文字颜色

你可以设置文本的颜色：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="color: tomato;">Hello world</h1>
>      <p style="color: dodgerblue;">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
>      <p style="color: mediumseagreen;">Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
>  </body>
> </html>
> ```



### 11.4 边框颜色

你可以为边框设置颜色：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="border: 2px solid tomato;">Hello World</h1>
>      <h1 style="border: 2px solid dodgerblue;">Hello World</h1>
>      <h1 style="border: 2px solid violet;">Hello World</h1>
>  </body>
> </html>
> ```



### 11.5 颜色值

在HTML中，颜色可以以RGB、HEX、HSL、RGBA、HSLA值来进行设置。一下三个元素就是通过不同的方式来设置相同的背景颜色：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="background-color: rgb(255, 99, 71);">rgb(255, 99, 71)</h1>
>      <h1 style="background-color: #ff6347;">#ff6347</h1>
>      <h1 style="background-color: hsl(9, 100%, 64%);">hsl(9, 100% 64%)</h1>
>  </body>
> </html>
> ```

以下两个元素是通过`RGBA` 和 `HSLA` 值进行设置，这两种都给颜色添加了一种淡化效果（在这里我们使用的是50%的程度）：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="background-color: rgba(255, 99, 71, 0.5);">rgba(255, 99, 71, 0.5)</h1>
>      <h1 style="background-color: hsla(9, 100%, 64%, 0.5);">hsla(9, 100%, 64%, 0.5)</h1>
>  </body>
> </html>
> ```



## 12. HTML 样式 - CSS

*CSS 的全称是 `级联样式表`，CSS可以为你节省一大笔工作。它可以一次性控制多个网页的布局。*



### 12.1 什么是CSS？

级联样式表（CSS）用来给网页的布局设置格式。

有了CSS，你可以控制颜色、字体、字体大小、元素之间的间隙、元素布置的位置、背景图或者背景色的使用以及为不同的设备或不同的窗口大小设置不同的展示方式等等等等！

**贴士**：级联的意思是父级元素的样式可以传给所有子级元素进行展示。因此，如果你设置一个body文字的颜色为蓝色，所有body内的头、段落以及其他文本元素可以以同样的颜色进行展示（除非你制定了别的样式）！



### 12.2 使用CSS

CSS可以在HTML文件中以三种方式进行使用：

* **行内** - 通过在HTML元素内使用 `style` 特性
* **内部** - 通过在`<head>` 标签内使用`<style>` 元素
* **外部** - 通过使用`<link>` 元素指向一个外部的CSS文件

通常添加CSS的方式是使用CSS文件存储所有的样式。然而，在本教程中我们将使用行内或者内部style样式，因为这样易于验证，易于自己亲自进行试验。



### 12.3 行内CSS

行内CSS可以用来为单个HTML元素添加独一的样式。

行内CSS可以使用为HTML元素使用 `style` 特性。

以下案例设置了 `<h1>` 元素的文本颜色为蓝色，以及`<p>` 元素的文本颜色为红色：

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <body>
>      <h1 style="color: blue;">A Blue Heading</h1>
>      <p style="color: red;">A red paragraph</p>
>  </body>
> </html>
> ```



### 12.4 内部CSS

一个内部CSS可以为单个HTML页面设置样式。

内部CSS可以被定义于HTML页面的`<head>` 区域内，使用一个 `<style>` 标签。

以下的案例将 `<h1>` 元素（页面顶上）的文字颜色改为蓝色，而所有 `<p>` 元素的文字颜色为红色，页面的背景色将为 `powderblue` 颜色。

> 案例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <style>
>          body {background-color: powderblue;}
>          h1 {color: blue;}
>          p {color: red;}
>      </style>
>  </head>
>  <body>
>      <h1>This is a heading.</h1>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```



### 12.5 外部CSS

一个外部CSS可以用来为多个HTML页面定义格式。

通过给每个HTML页面在 `<head>` 区域中添加一个链接来使用外部样式表。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <link rel="stylesheet" href="styles.CSS">
>  </head>
>  <body>
>      <h1>This is a heading.</h1>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```



外部样式表可以在其他的文字编辑器中编写。这个文件不能包含任何的HTML代码，而且必须以.CSS作为扩展名。

以下为案例：

> 范例：
>
> ```css
> body {
>  background-color: powderblue;
> }
> 
> h1 {
>  color: blue;
> }
> 
> p {
>  color: red;
> }
> ```

**贴士**：有了外部样式表，你可以通过仅改变一个文件来改变整个网站的样式。



### 12.6 CSS颜色，字体和大小

在这里，我们将演示一些常用的CSS属性，你可以在之后学到更多关于它的知识。

CSS `color` 属性定义了使用的文字颜色。

CSS `font-family` 属性定义了使用的字体。

CSS `font-size` 属性定义了文本的大小。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <style>
>          h1 {
>              color: blue;
>              font-family: Verdana, Geneva, Tahoma, sans-serif;
>              font-size: 300%;
>          }
> 
>          p {
>              color: red;
>              font-family: 'Courier New', Courier, monospace;
>              font-size: 160%;
>          }
>      </style>
>  </head>
>  <body>
>      <h1>This is a heading</h1>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```



### 12.7 CSS边境

CSS `border` 属性给HTML元素定义了一个边框。

**贴士**：你几乎可以给所有HTML元素添加边框。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <style>
>          p {
>              border: 2px solid powderblue;
>          }
>      </style>
>  </head>
>  <body>
>      <h1>This is a heading.</h1>
> 
>      <p>This is a paragraph.</p>
>      <p>This is a paragraph.</p>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```



### 12.8 CSS 内边距

CSS `padding` 属性用于定义内边距。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <style>
>          p {
>              border: 2px solid powderblue;
>              padding: 30px;
>          }
>      </style>
>  </head>
>  <body>
>      <h1>This is a heading.</h1>
> 
>      <p>This is a paragraph.</p>
>      <p>This is a paragraph.</p>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```



### 12.9 CSS 外边距

CSS `margin` 属性用于定义外边距。

> 范例：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <style>
>          p {
>              border: 2px solid powderblue;
>              margin: 50px;
>          }
>      </style>
>  </head>
>  <body>
>      <h1>This is a heading</h1>
> 
>      <p>This is a paragraph.</p>
>      <p>This is a paragraph.</p>
>      <p>This si a paragraph.</p>
>  </body>
> </html>
> ```



### 12.10 外部CSS样式链接

外部样式表可以通过一个全URL或者路径来给当前页面进行使用。

> 范例：
>
> 该案例使用了全URL去链接一个样式表：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
>  </head>
>  <body>
>      <h1>This is a heading</h1>
> 
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```

> 范例：
>
> 该案例通过定位当前网站中的文件夹来连接样式表：
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <link rel="stylesheet" href="/CSS/html/styles.CSS">
>  </head>
>  <body>
>      <h1>This is a heading.</h1>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```

> 范例：
>
> 该案例中的链接指向当前页面同一个文件夹的样式表
>
> ```html
> <!DOCTYPE html>
> <html>
>  <head>
>      <link rel="stylesheet" href="styles.CSS">
>  </head>
>  <body>
>      <h1>This is a heading</h1>
>      <p>This is a paragraph.</p>
>  </body>
> </html>
> ```



## 13. HTML 链接

*链接几乎可以在所有的网页中找到。链接允许用户去点击它们进行网页的跳转*



### 13.1 HTML 链接 - 超链接

HTML 链接都是超链接。

你可以通过点击链接来跳转到其他网页中。

当你将鼠标悬浮于链接上。鼠标指针将转换为一只小手。



### 13.2 HTML 链接 - 语法

HTML `<a>` 标签定义了一个超链接，它有如下语法：

> ```html
> <a href="url">link text</a>
> ```

`<a>` 元素中最重要的特性就是 `href` 特性，它表示链接的目的地。

而其中的 *link text* 则是在阅读器中可视的部分。

点击链接中的文字将给阅读器指向一个特定的URL地址。

> 范例：
>
> 该案例展示了如何制造一个指向 W3School.com 的链接：
>
> ```html
> <a href="https://ww.w3schools.com/">Visit W3Schools.com!</a>
> ```

默认情况下，链接将会展示以下部分到浏览器中：

* 一个未访问过的链接有下划线而且呈蓝色
* 一个已访问过的链接有下划线而且呈紫色
* 一个动态链接有下划线而且呈红色

> **贴士**：链接当然也能通过CSS被改变样式
