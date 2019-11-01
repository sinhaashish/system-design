---
layout: post
title:  如何使用system-design这个Jekyll模版
date:   2016-08-27 01:08:00 +0800
categories: document
tag: 教程
major: A
---

* content
{:toc}


致谢							{#Thanks}
====================================
+ 感谢[Less官网](http://lesscss.cn/)的样式，本Jekyll框架的样式都是基于Less官网的样式直接拷贝过来的。只是重构了JS，并且加入了Jekyll语法而已。
+ 感谢[Github](https://github.com/)提供的代码维护和发布平台
+ 感谢[Jekyll](https://jekyllrb.com/)团队做出如此优秀的产品
+ 感谢[Solar](https://github.com/mattvh/solar-theme-jekyll)的原作者[Matt Harzewski](http://www.webmaster-source.com/)，在`2014.11`-`2016.09`的两年间，我的博客选用了此样式模版


使用							{#How-to-use}
====================================

下载							{#Download}
------------------------------------

使用git从[system-design](https://github.com/sinhaashish/system-design.git)主页下载项目

```bash
git clone https://github.com/sinhaashish/system-design.git
```

配置							{#Configuration}
------------------------------------


Just use one file _config.yml to configure the system-design project. After opening it, configure as follows.

> Pay special attention to the configuration of `baseurl`. If it is a ***. The github.io project, if it is not modified to be empty, will cause errors such as JS, CSS, and other static resources not found.

``` Celebration
Name: Blog Name
Email: Email address
Author: Author Name
Website: Personal website
### baseurl changes to the project name if the project is '***. Github.io', set to empty ''
Baseurl: " / system-design"
Resume_site: Restore website
Github: github address
Github_username: github username
FB:
Comment:
Provided by duoshuo
Duoshuo:
Short_name: Say more accounts
Disqus:
Abbreviation: Disqus account
```

How to write an article {#How-to-write-document}
------------------------------------

在`system-design/_posts`目录下新建一个文件，可以创建文件夹并在文件夹中添加文件，方便维护。在新建文件中粘贴如下信息，并修改以下的`titile`,`date`,`categories`,`tag`的相关信息，添加`* content {:toc}`为目录相关信息，在进行正文书写前需要在目录和正文之间输入至少2行空行。然后按照正常的Markdown语法书写正文。

```bash
---
layout: post
#标题配置
title:  标题
#时间配置
date:   2016-08-27 01:08:00 +0800
#大类配置
categories: document
#小类配置
tag: 教程
---

* content
{:toc}


我是正文。我是正文。我是正文。我是正文。我是正文。我是正文。
```

执行							{#execute}
------------------------------------

```bash
jekyll server
```

效果							{#result}
------------------------------------
打开浏览器并输入URL`http://localhost:4000/`,回车。


为什么重复造轮子					{#why}
====================================

很明显，我在重复造轮子。在13年接触到GIT，14年末接触到Jekyll，然后搭建了自己的博客，当时是选用了[JekyllThemes](http://jekyllthemes.org/)上的[Solar](https://github.com/mattvh/solar-theme-jekyll)主题，一直到现在。不过中间一直感觉页面风格还是偏暗，阅读不方便。并且有一些小的细节做的不是很好。在页面的跨平台浏览上有一些瑕疵。并且不区分一级标题和二级标题，导致没有重点强调。诸如此类，用了2年，用的越多，越发吃力，中间就一直在寻找新的能够让我一眼认定的主题。

虽然设计好看的主题很多。但是真正适合拿来做博客的却不多。中间一直没有找到合适的主题。直到有一天看到Less官网的主题之后，豁然觉得这就是我的博客想要的样子。简单而又不平凡。所以就决定了要把博客迁移到这个主题，然后拿了两天晚上来把这个主题做出来。

重复造了轮子，但是这个是迄今为止自己觉得最适合我的博客的轮子，所以是值得的！

关于作者						{#about-author}
====================================

热爱开源，热爱折腾的Java程序猿。更多个人信息和联系方式可以参照[我的简介](http://www.hifreud.com/Resume.io/)。
