# 前后端分离
 
 ## 前后端分离的历史
软件开发早期是没有前后端分离的概念的，为什么？因为当时压根儿就没有前端工程师，专门的前端工程师大约是在2005年。在此之前前端是不受重视的。这其实和软件的发展有关，说到这里又不得不提到js的发展历史。JavaScript诞生于1995年。起初它的主要目的是处理以前由服务器端负责的一些表单验证。后来大家对页面的要求越来越高，js又给web多了一些动态功能。大家对前端的需求就是展示静态内容或者简单的动态内容（比如CGI返回数据拼接输出“动态”内容）

## 前后端分离
1998年ajax技术的出现，允许客户端脚本发送HTTP请求（XMLHTTP），并且局部刷新页面，这种突破性的创新使得web高速发展，推动了web的发展。随着HTML5，CSS3，ES6（简称356）的出现，web正以前所未有的速度前进，web工程师从无到有，再到现在web工程师被赋予了很多花环，机遇和挑战。也因此前后端不得不逐渐的分离。
## 前后端合并
正所谓合久必分，分久必合。 前几年被热炒的全栈工程师，以及前后端同构技术都反映了前端端在分离之后又逐渐合并的迹象。为什么会这样呢？前后端分离虽然减少了后端开发的工作（最初前端都是后端写的，比如.net 的 aspx  java的jsp等）。但前后端分离地不干净导致一些沟通问题反而不如一个人来做。为了解决这个问题，主要又两种方式：
* 全栈工程师。 将所有工作交给一个人，或者有着前后端知识的一群人，这样沟通起来成本比较低。
* 稍后讲。
## 那还又必要分离吗？
上面讲述了前后端合并，那么还有必要分离吗？ 非常又必要！！！

刚才说为了解决前后端沟通问题主要又两种方式，下面说下第二种。

* 建立中间层。 前后端问题产生的原因主要是两个，一个是知识背景，技术栈不同，难以互相理解。二是 前后端是一个依赖的关系，前端需要依赖后端的数据接口，因此存在工作上的先后关系。 建立中间层可以有效减少上述的问题。 目前淘宝，挖财，51，有赞，二维火都在尝试这种方式。这也是我将会在后面重点描述的方式。

最近出现的docker容器技术等有效地减少了后端的工作量，让后端更加专注业务逻辑的编写。我觉得node的出现也大概如此吧，它的出现不是用来替代apache成为下一个web容器，我觉得他更是扩展了前端的领域，使得可以将一部分后端无法做（比如ssr）或者不好做（不愿意做）的东西（比如接口聚合），移交给前端。


> 我不喜欢被冠以前端工程师，后端工程师的帽子。 我喜欢工程师这个称呼，我觉得我是以工程化的方式解决问题的角色，而不应该限定于某一部分职责。这个我主张前后端分离不矛盾，每个角色都自己的分工，都有自己精细化的一面。我们不试图取代后端，我们只是专注做好自己罢了。