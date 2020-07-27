# CSS 盒模型

## 1、什么是盒模型？

​	盒子模型（Box Model）就是把HTML页面中的元素看作是一个矩形的盒子，也就是一个盛装内容的容器。每个矩形都由元素的**内容(content)、内边距（padding）、边框（border）和外边距（margin）**组成。**每个盒子除了有自己大小和位置外，还影响着其他盒子的大小和位置。**

　　**盒子模型特性：**

- 每个盒子都有：边界、边框、填充、内容 4个属性；
- 每个属性都包括4个部分：上、右、下、左。属性的4部分可以同时设置，也可以分别设置。

## 2、标准盒模型与怪异盒模型的表现效果的区别

​	**1）标准盒模型**中**width**指的是内容区域**content**的宽度；**height**指的是内容区域**content**的高度。

​	**标准盒模型下盒子的大小**  = **content** + **padding** + **border** + **margin**

![img](https://img2018.cnblogs.com/blog/1748092/201908/1748092-20190809145641572-714793117.jpg)

 	**2）怪异盒模型**中的**width**指的是内容、边框、内边距总的宽度（content + padding+ border ）；**height**指的是内容、内边距、边框总的高度。

​	**怪异盒模型下盒子的大小=width（content + border + padding） + margin**

​	**![img](https://img2018.cnblogs.com/blog/1748092/201908/1748092-20190809145529154-1986045519.jpg)**

------

 **3）如何选择盒模型**

​	如果是定义了完整的doctype的标准文档类型，无论是哪种模型情况，最终都会触发标准模式。

​	如果doctype协议缺失，会由浏览器自己界定，在IE浏览器中IE9以下（IE6.IE7.IE8）的版本触发怪异模式，其他浏览器中会默认为W3c标准模式。

## 3、CSS3的box-sizing

box-sizing语法：

    box-sizing ： content-box || border-box || inherit;
    
    当设置为box-sizing:content-box时，将采用标准模式解析计算，也是默认模式；
    
    当设置为box-sizing:border-box时，将采用怪异模式解析计算。

