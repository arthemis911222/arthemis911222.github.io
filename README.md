## Leaf Blog

[**view the blog ->**](https://arthemis911222.github.io)

Forked from the Hux Blog.

---

#### Deploy Blog

搭建Git Page博客 ->
[EN](https://github.com/Huxpro/huxpro.github.io) | [中文](https://github.com/Huxpro/huxpro.github.io/blob/master/README.zh.md)


#### Deploy Comment
添加评论区 ->

2019年09月05日更新：
因为gitment评论区出现问题，在试过几个解决方案后，决定换成gitalk。

替换：[gitalk](https://github.com/gitalk/gitalk)

弃用：[gitment](https://github.com/imsun/gitment)

**【以下为gitment的部署方式和问题解决，目前已不可用，留作参考记录。】**

部署过程可参考 -> [在Jekyll博客添加评论系统：gitment篇](https://www.cnblogs.com/jacobpan/archive/2017/07/18/7200512.html)

因为gitment已经关闭，不再维护，所以初始化评论的时候回报错“object ProgressEvent”。解决方法请参考这里：[gitment issue 170](https://github.com/imsun/gitment/issues/170)

我是参考这篇[博客](https://awen.me/post/64465.html)，将 layouts 文件夹下的 post.html 文件做以下修改：


```html
<link rel="stylesheet" href="https://imsun.github.io/gitment/style/default.css">
<script src="https://imsun.github.io/gitment/dist/gitment.browser.js"></script>
```
改为：

```html
<link rel="stylesheet" href="https://imsun.github.io/gitment/style/default.css">
<script src="https://file.awen.me/gitment.browser.js"></script>
```

当然，最好的方法还是在自己的服务器 git clone 原来的 gitment 项目，然后自己启一个。遗憾的是，我没有服务器（之前的学生服务器也被释放掉了），也许可以期待实验室给一个（做梦中）？
