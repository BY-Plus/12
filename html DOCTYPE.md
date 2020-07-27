# DOCTYPE

## 1、什么是DOCTYPE?

​	DOCTYPE是document type的简写，它并不是 HTML 标签，也没有结束标签，它是一种标记语言的文档类型声明，即告诉浏览器当前 HTML 是用什么版本编写的。

​	注意: DOCTYPE的声明必须是 HTML 文档的第一行，位于html标签之前。大多数Web文档的顶部都有doctype声明，它是在新建一个文档时，由Web创作软件草率处理的众多细节之一。很少人会去注意 doctype ，但在遵循标准的任何Web文档中，它都是一项必需的元素。doctype会影响代码验证，并决定了浏览器最终如何显示你的 Web文档。


## 2、DOCTYPE的作用

声明文档的解析类型(document.compatMode)，避免浏览器的怪异模式。

​	**document.compatMode：**

​		**BackCompat：怪异模式，浏览器使用自己的怪异模式解析渲染页面。**

​		**CSS1Compat：标准模式，浏览器使用W3C的标准解析渲染页面。**

 	这个属性会被浏览器识别并使用，但是如果你的页面没有DOCTYPE的声明，那么compatMode默认就是BackCompat，浏览器按照自己的方式解析渲染页面，那么，在不同的浏览器就会显示不同的样式。

​    如果你的页面添加了<!DOCTYPE html>那么，那么就等同于开启了标准模式，那么**浏览器就得老老实实的按照W3C的标准解析渲染页面**，这样一来，你的页面在所有的浏览器里显示的就都是一个样子了。

## 3、DOCTYPE的取值

```
HTML 5： 

<!DOCTYPE html>

HTML 4.01 Strict

该 DTD 包含所有 HTML 元素和属性，但不包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">

HTML 4.01 Transitional

该 DTD 包含所有 HTML 元素和属性，包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">

HTML 4.01 Frameset

该 DTD 等同于 HTML 4.01 Transitional，但允许框架集内容。

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd">

XHTML 1.0 Strict

该 DTD 包含所有 HTML 元素和属性，但不包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。必须以格式正确的 XML 来编写标记。

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">

XHTML 1.0 Transitional

该 DTD 包含所有 HTML 元素和属性，包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。必须以格式正确的 XML 来编写标记。

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" " http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

XHTML 1.0 Frameset

该 DTD 等同于 XHTML 1.0 Transitional，但允许框架集内容。

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">

XHTML 1.1

该 DTD 等同于 XHTML 1.0 Strict，但允许添加模型（例如提供对东亚语系的 ruby 支持）。

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
```

