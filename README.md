**首先，这是一个“不严谨”的项目**

<br>

起因是，我最近喜欢用Twitter家的Bootstrap 5来写Web页面。

但是Bootstrap官方目前没有做dark mode，然而我又想要dark mode. 于是我找到了这么个项目：https://github.com/vinorodrigues/bootstrap-dark-5

于是问题解决了，但又没完全解决。这个项目的样式，并不是我想要的深色模式，而是夜间模式。

深色模式和夜间模式有区别的啊。

<br><br>

------

<br>

这个项目也很不严谨，它的原理就是在bootstrap-dark-5的css后面再加载一个css文件来覆盖掉原有的一些样式（主要是配色）。

于是项目本身也挺简单的，我没用scss也没用npm啥的，就是一个.net 工程，构建的时候会自动生成 min.css

使用的话，把 min.css复制到想要的地方完事了。

<br>

**为什么是 .NET 工程：**

因为我开发机上正好有 .net sdk， 然后 .net 可以热重载，我写css的时候不需要手动重启项目或者刷新浏览器。

**那为什么不用npm**

因为没必要，就一个css文件而已。