# VeryLess 2.0
http://veryless.org

VeryLess是基于LESS的Mixin扩展库,由LESS中国社区( http://lesscss.net/ )发起。<br>
提供一系列方法库，帮助我们快速敏捷的编写样式。

## 使用方法
	
安装veryless
	
	npm install -g veryless

Usage:

	初始化  目录: veryless -init ./myfolder
	下载 Plugin:
	cd myfolder
	veryless -use pluginname
	就会下载对应的插件到 ./myfolder/veryless/pulgins/里


或者可以直接下载veryless.less到本地使用: https://github.com/feichang/veryless/blob/master/veryless.less

举个栗子：
	
	我的项目目录：/mysite
	我的前端资源文件：/mysite/assets
	sudo npm install -g veryless
	cd /mysite
	# 初始化 目录
	veryless -init assets
	# 下载Plugin css3
	veryless -use css3 assets

## API文档

https://github.com/feichang/veryless/tree/master/api

## 分层说明

*  Base        

	提供全局Reset和一些Reset方法，比如reset字体颜色、大小等等
*  Compatible

	提供常用浏览器兼容解决方案，如png24透明的问题，比如fixed定位问题
*  Util

	提供常用的工具方法，能够加快开发速度，如清楚浮动clearfix, 如Retina屏幕高清图片支持等
*  Layout

	提供常用的布局方法，目前有绝对栅格布局，流式布局，Metro风格布局

*  Shortcut

	提供常用的快捷写法，如font-size: 12px; 可以写成： .font-s12;或者 .font-s(12px);
*  Plugin
	
	存放第三方插件，如[css3.less],[animation.less],[brand-color.less]

## Plugin介绍

VeryLess提供了Plugin概念，任何人都可以利用Veryless创建属于自己的plugin&使用plugin。

## 如何开发Plugin

1, Fork veryless  https://github.com/feichang/veryless

2, 将自己的Plugin提交到fork到个人Github上的veryless中plugins文件夹中

3, Pull request

4, 审核通过后，用户可以通过 veryless -use pluginname path 的方式使用

## Plugin规范

	/Plugins/yourplugin
	index.less 这里存放plugin的所有代码（注意：一定要是index.less）
	README.md  介绍你的plugin

## 作者

* 飞长
	* 微博：@非常长
	* http://veryued.org

* TooBug
    * 微博：@Toobug
    * http://www.toobug.net/

## Plugin 列表 & 她的作者们

### CSS3

* 描述：提供一些CSS3快捷方式
* 文档地址：https://github.com/feichang/veryless/tree/master/plugins/css3
* 作者：飞长
* 微博：@非常长
* blog: http://veryued.org
* github: https://github.com/feichang

### Animation

* 描述：提供一些Animation的方法
* 文档地址：https://github.com/feichang/veryless/tree/master/plugins/animation
* 微博：@非常长
* blog: http://veryued.org
* github: https://github.com/feichang

### BrandColor

* 描述：提供各大公司的标准颜色
* 文档地址：http://veryless.org/veryless/test/ui/color/color.html
* 微博：@非常长
* blog: http://veryued.org
* github: https://github.com/feichang

### Waterflow

* 描述：瀑布流布局
* 文档地址：https://github.com/feichang/veryless/tree/master/plugins/waterfall
* 作者：moe
* 微博：@刘剑锋_moe
* blog: www.moejser.com
* github: https://github.com/fengliu222
