Welcome to Bootstrap StepWizard!
===================


bootstrap_stepwizard 是一个基于bootstrap2.3开发的步进分页组件

    This project is moving from GitHub.
 

 - [Click here to view the dome page(Link to GitHub)](http://eastpiger.github.io/bootstrap_stepwizard/)
 - [中文Dome页面（导向GitHub）](http://eastpiger.github.io/bootstrap_stepwizard/introcn.html)
 - [English](http://eastpiger.github.io/bootstrap_stepwizard/introcn.html)

----------


介绍
-------------

有时候我们需要一个能够提供步骤前后关联的导航插件，曾经有一些项目用来实现，**但是**都很难使用。

所幸，Bootstrap StepWizard这个新项目仅仅用3kb的文件就可以实现像***Bootstrap_Tabs.js***一样好用的东西，就像这样：
![SnapShot](http://git.geekpie.org/eastpiger/bootstrap_stepwizard/raw/master/SnapShot.jpeg)


下载
-------------

这个项目包含两个主要文件： ***bootstrap_stepwizard.js*** 和 ***bootstrap_stepwizard.css***。或者使用压缩后的版本： ***bootstrap_stepwizard.min.js*** 和 ***bootstrap_stepwizard.min.css*** 。

GitLab下载地址： http://git.geekpie.org/eastpiger/bootstrap_stepwizard



安装
-------------
> **Note:**

> - 这个项目依赖于bootstrap 和 Jquery，您需要先安装上述工具。

安装Bootstrap StepWizard只需把以下代码插入网页的合适位置：

    <link href="bootstrap_stepwizard.css" rel="stylesheet" media="screen">
	<script src="bootstrap_stepwizard.js"></script>


用法
-------------
显示Bootstrap StepWizard只需在需要的位置输入以下代码：


    <ul class="nav nav-stepwizard" id="myStepWizard_show">
		<li class="complete"><span href="#home" data-toggle="tab"><span class="badge">1</span>Home</span></li>
		<li class="active"><span href="#profile" data-toggle="tab"><span class="badge">2</span>Profile</span></li>
		<li><span href="#messages" data-toggle="tab"><span class="badge">3</span>Messages</span></li>
		<li><span href="#settings" data-toggle="tab"><span class="badge">4</span>Settings</span></li>
	</ul>
	<div class="tab-content">
		<div class="tab-pane active fade in" id="home">Home is a home.</div>
		<div class="tab-pane fade" id="profile">Profile can see the profile.</div>
		<div class="tab-pane fade" id="messages">Message allows you to send messages.</div>
		<div class="tab-pane fade" id="settings">Settings ... just as you know.</div>
	</div>

> **Note:**

> - 你可能发现了，这里的代码和使用 ***bootstrap-tab.js***（可切换式标签页）几乎一样，仅仅把 **nav-tabs** 换成了 **nav-stepwizard** 。

如果您不希望用户可以点击标签自行切换（就像上面的实例那样），只需再添加 **nav-stepwizard_unabled** 到#myStepWizard_show上即可。

    <ul class="nav nav-stepwizard nav-stepwizard_unabled" id="myStepWizard_show">

JavaScript
-------------

项目提供了一些js函数，您可以在js或Jquery中使用。

    <link href="bootstrap_stepwizard.css" rel="stylesheet" media="screen">
	<script src="bootstrap_stepwizard.js"></script>


**stepwizard_prev function 前一项跳转**

	function stepwizard_prev(handle)
实例：

	$("#pre_show").click(function(){
		stepwizard_prev($("#myStepWizard_show"));
	});	
当前位于第一个时返回-1。

**stepwizard_next function 后一项跳转**

	function stepwizard_next(handle)
实例：

	$("#next_show").click(function(){
		stepwizard_next($("#myStepWizard_show"));
	});
当前位于最后一个时返回-1。

**stepwizard_to function 指定index项跳转**

	function stepwizard_to(handle,index)
实例：

	$("#index_jump").click(function(){
		stepwizard_to($("#myStepWizard_show"),3);
	});
指定index不存在时返回-1。


**stepwizard_index function 当前项index查询**

	function stepwizard_index(handle)
实例：

	$("#index_show").click(function(){
		alert(stepwizard_index($("#myStepWizard_show")));
	});
返回当前项index。


关于
-------------
欢迎访问我的主页***[www.eastpiger.com](www.eastpiger.com)***
