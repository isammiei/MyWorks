### 包含内容

修饰线，首行缩进，行高，font 属性复合写法，内容水平居中，字间距，字符间距   
## text-decoration属性-修饰线
用于设置文本的修饰线外观的（下划线、上划线、贯穿线/删除线 或 闪烁）
常用的属性值有以下三种  
none没有修饰线
underline下划线
line-through删除线  
### 扩展延伸：

text-decoration 它是以下四个属性的简写

text-decoration-line ：文本修饰的位置，如下划线underline，删除线line-through
text-decoration-color：文本修饰的颜色
text-decoration-style：文本修饰的样式，如波浪线wavy实线solid虚线dashed
text-decoration-thickness：文本修饰线的粗细 
## text-indent属性-首行缩进
### 首行缩进
text-indent 属性定义首行文本内容之前的缩进量
比如：中文一般文章书写都会 缩进两个字符
常用单位是em，1em是一个字符的宽度,2em表示 2 个字符的宽度    
## line-height属性-行高
### 行高

line-height 属性定义行高
如何测量行高，有很多种方式，比如：从一行文字的最顶部到下一行文字的最顶部之间的距离，就是行高。  
### 关于行高的最佳实践
line-height 属性的单位可以是 px 为单位的数值
line-height 属性也可以是没有单位的数值，表示字号的倍数，这是最推荐的写法
实际工作中行高：1.25 , 1.5 , 1.75 都是常用的倍数设置
line-height 属性也可以是百分数，表示字号的倍数  
line-height - CSS（层叠样式表） | MDN
<https://developer.mozilla.org/zh-CN/docs/Web/CSS/line-height>  
### 注：

推荐在设置 line-height 时使用无单位数值
主段落内容的 line-height 至少应为 1.5
如果文字的大小要随页面的缩放而变化，请使用无单位的值，以确保行高也会等比例缩放。    

## 行文本垂直、水平居中
① 行文本垂直居中

设置 行高 = 盒子高度 ，即可实现单行文本垂直居中 
② text-align 属性

定义 行内内容（例如文字、图片、行内块级元素） 相对它的块父元素的对齐方式
常用的三个属性值：

left 水平居左
right 水平居右
center 水平居中 

## font合写属性-复合写法
font 属性可以用来作为 font-style，font-weight ，font-size ，line-height 和 font-family 属性的合写   
### font 属性连写注意事项

font 属性连写时，必须设置 font-size 和 font-family 才能生效
连写时，行高问题    
font-style和font-weight 必须在 font-size 之前   

## 继承性
关于文字属性的继承性和就近原则  
① 祖先元素设置，后代元素即生效
文本相关的属性普遍具有继承性，只需要给 祖先标签 设置，即可在后代所有标签中生效  
因为文字相关属性有继承性，所以通常会设置 <body>标签的字号、颜色、行高等，这样就能当做整个网页的默认样式了   
② 就近原则
在继承的情况下，选择器权重计算失效，而不是就近原则  
在继承的情况下，选择器权重计算失效，而是就近原则    

## word-spacing字间距
word-spacing 表示字间距，对中文是无效的，仅对英文字单词起作用   
normal, 长度    
## letter-spacing字符间距
letter-spacing 属性用于设置文本字符的间距表现。 
normal, 长度