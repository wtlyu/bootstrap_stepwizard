Welcome to Bootstrap StepWizard!
===================


bootstrap_stepwizard is a StepWizard for bootstrap 2.3

    This project is moving from GitHub.
 

 - [Click here to view the dome page(Link to GitHub)](http://eastpiger.github.io/bootstrap_stepwizard/)
 - [中文Dome页面（导向GitHub）](http://eastpiger.github.io/bootstrap_stepwizard/introcn.html)
 - [中文说明页面](http://eastpiger.github.io/bootstrap_stepwizard/introcn.html)

----------


Introduce
-------------

Sometimes I want to use the tabs of bootstrap just like a step wizard . There used to be many project to do it such as Fuel UX and many others **but** very difficult to use .

Fortunately , Bootstrap StepWizard is a new project within 3kb files to do it easily just like using ***Bootstrap_Tabs.js*** . like this :
![SnapShot](http://git.geekpie.org/eastpiger/bootstrap_stepwizard/raw/master/SnapShot.jpeg)


Download
-------------

This project contains two major file : ***bootstrap_stepwizard.js*** and ***bootstrap_stepwizard.css*** . You can also use its packed edition : ***bootstrap_stepwizard.min.js*** and ***bootstrap_stepwizard.min.css*** .

You can download the project via GitLab : http://git.geekpie.org/eastpiger/bootstrap_stepwizard



Install
-------------
> **Note:**

> - This project has reliance on bootstrap and Jquery and you should install them firstly .

To install Bootstrap StepWizard , you should type this in your webpage :

    <link href="bootstrap_stepwizard.css" rel="stylesheet" media="screen">
	<script src="bootstrap_stepwizard.js"></script>


Usage
-------------
To show Bootstrap StepWizard in your page , you can just type this in your webpage :


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

> - It is similer to use ***bootstrap-tab.js*** . Just replace **nav-tabs** into **nav-stepwizard** .

If you don't want users to click the button ( just like the example above ) , Just add a class **nav-stepwizard_unabled** .

    <ul class="nav nav-stepwizard nav-stepwizard_unabled" id="myStepWizard_show">

JavaScript
-------------

This project alse contains some js functions . you can use them in js or Jquery .

    <link href="bootstrap_stepwizard.css" rel="stylesheet" media="screen">
	<script src="bootstrap_stepwizard.js"></script>


**stepwizard_prev function**

	function stepwizard_prev(handle)
example:

	$("#pre_show").click(function(){
		stepwizard_prev($("#myStepWizard_show"));
	});	
It returns -1 when the active tab is the first .

**stepwizard_next function**

	function stepwizard_next(handle)
example:

	$("#next_show").click(function(){
		stepwizard_next($("#myStepWizard_show"));
	});
It returns -1 when the active tab is the last .

**stepwizard_to function**

	function stepwizard_to(handle,index)
example:

	$("#index_jump").click(function(){
		stepwizard_to($("#myStepWizard_show"),3);
	});
It returns -1 when the target index is unabled .


**stepwizard_index function**

	function stepwizard_index(handle)
example:

	$("#index_show").click(function(){
		alert(stepwizard_index($("#myStepWizard_show")));
	});
It returns the active index .


About
-------------
Welcome to my homepage at ***[www.eastpiger.com](www.eastpiger.com)***
