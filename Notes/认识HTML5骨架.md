### 1. 文档类型声明DTD  

#### 定义和用法

<!DOCTYPE> 声明必须是 HTML 文档的第一行，位于 <html> 标签之前。 
<!DOCTYPE> 声明不是 HTML 标签，它是指示 web 浏览器关于页面使用哪个 HTML 版本进行编写的指令。    
在 HTML 4.01 中，<!DOCTYPE> 声明引用 DTD，因为 HTML 4.01 基于 SGML。DTD 规定了标记语言的规则，这样浏览器才能正确地呈现内容。    

#### SGML（Standard Generalized Markup Language）    

即标准通用标记语言) SGML 是国际上定义电子文档和内容描述的标准。 
HTML5 不基于 SGML，所以不需要引用 DTD   

#### 提示：  

请始终向 HTML 文档添加 <!DOCTYPE> 声明，这样浏览器才能获知文档类型。    

不写 DTD 会引发浏览器的一些兼容问题
不同版本的 HTML 有不同的 DTD 写法 

#### HTML 4.01 与 HTML5 之间的差异   

在 HTML 4.01 中有三种 <!DOCTYPE> 声明。
在 HTML5 中只有一种 

### 2. W3C组织  
W3C 指万维网联盟（World Wide Web Consortium）是万维网的主要国际标准组织 
W3C 创建于 1994 年 10 月主要负责制定 WEB 标准   
W3C 由 Tim Berners-Lee（蒂姆·伯纳斯·李） 创建 ，被誉为 "互联网之父" 
W3C 是一个会员组织  
W3C 的工作是对 web 进行标准化   
W3C 创建并维护 WWW 标准 
W3C 标准也被称为 W3C 规范   
主要是 HTML 和 CSS  
W3C 组织官网：<https://www.w3.org/> 

JavaScript 由 Brendan Eich 于 1995 年发明，并于 1997 年成为 ECMA 标准。 

### 3. 网页组成 
网页主要由三部分组成：  

结构（Structure）、表现（Presentation）和行为（Behavior）   
结构：用于对网页元素进行整理和分类，即当下学习的 HTML   
表现：表现用户设置网页元素的排版、颜色、大小修饰等外观样式，即 CSS  
行为：行为是指网页模型的定义、交互等编写，即要学习的 JavaScript 

Web 标准提出的最佳体验方案：    

结构、样式、行为相分离  
即：结构写在 HTML 文件中，表现写在 CSS 文件中，行为写在 JavaScript 文件中   

### 4. HTML标签 
```
<!--文档类型声明-->
<!DOCTYPE html>
<!--
    <html></html>标签
    lang 表示网页的语言，en表示英语，zh表示中文 ,不修改也行
    什么时候修改呢：如果网站有多国语言时修改，中文版、英语版、日语版、法语版等等，具体案例可参考 小米官网源码
-->
<html lang="en">
  <!-- <head></head>标签对，是网页的配置，不要认为是网页的头部 -->
  <head> </head>
  <!-- <body></body>标签对中书写网页的内容，包括网页的头部、主要内容、页脚等各个部分 -->
  <body></body>
</html>
```
### 5. 字符集   
meta 元标签，表示网页的基础配置 
charset 字符集  
UTF-8 是一种字符集  
```
<meta charset="UTF-8" />
```
在中国常见的字符集有两种 UTF-8 和 gb2312    

无论使用哪种字符集，一定要在 Vscode 中将文件也设置为相同的字符集，否则会出现乱码    

Live Serve 插件不支持 gb2312、gbk 字符集，只支持 UTF-8 字符集

文件编码集与 meta 标签编码不一致网页会出现乱码  

同样的内容，不同的编码所占字节数也不同  

### 6. 网页三要素   

title：网页的标题（30 字以内）
文字会显示在浏览器的标题栏上
title 也是搜索引擎收录网站时显示的标题，为了吸引用户点击，合理的标题设置有利于 SEO 优化 
keywords：网页的关键词（关键词之间用英文状态下的逗号 "," 分隔） 
description：网页的描述（150 字以内）

SEO（Search Engine Optimization）即：搜索引擎优化

利用搜索引擎的规则提高网站在有关搜索引擎内的自然排名。目的是让其在行业内占据领先地位，获得品牌收益。    

### 7. VSCode 中 HTML 模板代码解读  
```
<!--声明当前文档类型为 html5标准-->
<!DOCTYPE html>
<!--声明当前页面的语言类型-->
<html lang="en">
  <head>
    <!--网页的编码集-->
    <meta charset="UTF-8" />
    <!--IE8及以上的版本按照最新的标准去渲染-->
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <!--用户移动端适配-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!--网页标题-->
    <title>艾编程</title>
    <!--网页关键词-->
    <meta name="Keywords" content="艾编程,WEB前端,Java架构师,Python课程" />
    <!--网页描述-->
    <meta name="description" content="为每个互联网人提供高质量的终身学习平台" />
  </head>
  <body></body>
</html>
```

