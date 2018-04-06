---
title: 制作自己的Chrome主题--主题创建者
date: 2018-04-06 15:47:36
categories: 
	- 技术
	- 小工具
tags: 
	- 小工具
	- 主题
	- Chrome
	- 主题美化
toc: true
---

这篇文章介绍一下一个制作Chrome主题的扩展应用——主题创建者。相信大多数人都想给自己的Chrome换上一个好看的主题，可是在主题商店找不到自己想要的便萌生了自己做的念头，无奈自己又没有制作主题的技术（流下没有技术的泪水.jpg）。那么，本文介绍的就是一个制作主题的简单途径。

<!--more-->
{% raw %}
<link rel="stylesheet" href="https://resource.rurilove.moe/statics/aplayer/APlayer.min.css">
<script src="https://resource.rurilove.moe/statics/aplayer/APlayer.min.js"></script>
<div id="player" class="aplyer" style="width: 100%;margin: auto "></div>
<script type="text/javascript">
	var ap = new APlayer({ 
	    element: document.getElementById('player'), 
	    narrow: false, 
	    autoplay: true, 
	    showlrc: false, 
	    music: { 
	        title: '神のまにまに', 
	        author: '初音ミク', 
	        url: 'https://resource.rurilove.moe/musics/02.mp3', 
	        pic: 'https://resource.rurilove.moe/images/mufront/02.jpg' 
	    } 
	}); 
	ap.init(); 
</script>
{% endraw %}
### 写在前面
这个扩展是我大约两年前刚刚适应了翻墙逛Google等网站的时候在Chrome扩展商店偶然发现的，当时就做了一些主题。去年的时候我想把原来的主题改善一下，突然发现在扩展商店找不到这款应用了（“主题创建者”的类型为Chrome**应用**，而不是扩展）。不仅如此，商店上`应用`这个分类全部消失了！！！

不过，好在我一直有备份的习惯，开始在我的众多U盘上寻找。最终在一个因不明原因分区全部消失的U盘的数据中找到了这个扩展的备份——一个zip压缩包。离线安装过chrome扩展的人应该了解Chrome扩展的安装文件应该是`.crx`后缀的，而且chrome可以直接打包。

我当时为什么不打包呢。当时我发现，这个扩展如果做成`.crx`Chrome会在安装的时候提示`只能通过Chrome网上应用店添加该程序`，所以只能用开发者模式运行。不过用开发者模式，每次开启Chrome就会有一个警告，很是烦人。于是我做了一个魔改版并且打包，应该可以绕过这个机制。**文章结尾会提供下载。**

那么先看看我的主题：
[![01.png](https://i.yusa.me/EBf1E4RnRAan.png "点击下载")](https://resource.rurilove.moe/DownLoad/theme1.crx)

### 正文
那么以下就是正文了。

#### 下载&&安装“主题创建者”
Chrome已经下架这些应用，不过目前版本的Chrome还是可以用已经下载的。

1. 下载我在本文最后提供的魔改版，可以得到一个`.crx`文件。
2. 打开 ` Chrome -> 菜单（工具）-> 更多工具 -> 扩展程序` 。
> ![02.png](https://i.yusa.me/LJfejJALxagz.png)

3. 将`.crx`文件拖放进去，安装完成。

#### 制作主题
在Chrome标题栏的左下方有一个 `应用` 的入口。你也可以在`开始菜单 -> Chrome应用 ` （如果你用的是Windows系统的话，Linux直接在启动器搜索）找到 `主题创建者` 。点击进入可以得到这个界面（其实已经设置为安装时自动开启）：
![03.png](https://i.yusa.me/WKiGEo8KJyb4.png)

当你将鼠标指针悬停在右侧各栏的上方时，会有一个指针指在左侧窗口的对应位置，然后点击选择你要使用的图片或颜色即可。

制作完成后，点击下方的这个 ![04.png](https://i.yusa.me/e8U9jX0a2Pbj.png)，会下载一个压缩包。根据提示找到并解压后，将解压得到的文件夹拖放到`扩展程序`中，即可应用主题。

#### 主题打包
不过这样有可能会触发前面提到的`开发者模式`警告。我们可以将主题打包。
1. 进入`扩展程序`，开启`开发者模式`。
2. 选择`打包扩展程序`，弹出如下窗口。
![05.png](https://i.yusa.me/32Cprqb0NwxY.png)
3. 点击`扩展程序根目录`，找到并选择主题的解压目录。
4. 打包！
5. 然后你就可以在之前解压主题的目录同目录下发现多出一个`.crx`文件。把它拖放到`扩展程序`试试吧。
6. 最后，最好还是把开发者模式关掉吧。

#### 使用
用上了自己的主题是不是感觉心里美滋滋的呢。还没有用Chrome浏览器的同学们也投入Chrome的大家庭中来吧。Chrome可是全世界最好的网页浏览器呢！**Chrome大法好！**

### 下载
Hugefiver魔改版主题创建者：[下载](https://resource.rurilove.moe/DownLoad/Chrome_Theme_Creator.crx)

**转载请标明原作者，并提供原文链接。**