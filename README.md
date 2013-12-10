﻿Dwarf Site Builder
==================

该项目通过特定的模板规则和Markdown插件生成纯静态的文档类内容站点。

Usage
-----

下载项目：

	$ git clone https://github.com/mytharcher/dwarf.git

### 命令行方式 ###

在命令行运行PHP脚本：
	
	$ cd path/to/dwarf
	$ mkdir output && chmod 777 output
	$ php build.php -p example -o output

### Web方式 ###

0.	下载仓库代码到本地Apache服务器下（最好建一个虚拟站点）。

0.  在浏览器中访问以下地址触发站点生成操作：
	
		http://yourhost/build.php?p=<project path>&o=<output path>

	以上`path`均为相对路径。需要确保`output path`目录存在且服务器有写权限。不需要加前置和结尾的`/`。

站点的模板语法和结构参见`example`目录。

History
-------

矮人在有和精灵一起的剧情里，总是以一种干吃苦活的次要身份出现。

在[elf+js]项目里，用于构建官方网站的这个程序就是这样。在了解github上可以使用更强大的[jekyll](http://github.com/mojombo/jekyll)之前，由于受不了一个一个页面构建的痛苦，然后就开发了这个构建脚本。等站点开发完，才发现原来github早就集成了jekyll，版本控制不说，加上全程托管和域名指向，什么都可以搞定了，根本不用我在这费事。

不过说回来，为什么要放弃自己写过的东西呢？虽然看起来每个轮子都差不多，但总和别人的有那么一点不一样。即使写的再烂，也是自己的，何况还有点用呢。

所以就放在这了，刚好作为[elf+js][]网站的第一版的纪念。**Dwarf**这个名字倒是临时想的，正好就当个elf的龙套了。也许哪天我又有新的想法，会再来升级的。

[elf+js]: http://elfjs.com/
