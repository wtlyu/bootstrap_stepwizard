bootstrap_stepwizard
====================

bootstrap_stepwizard is a StepWizard with bootstrap

<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="chrome=1">
		<title>Bootstrap_StepWizard</title>		
		<link href="http://libs.baidu.com/bootstrap/2.3.2/css/bootstrap.min.css" rel="stylesheet" media="screen">
		<link href="bootstrap_stepwizard.css" rel="stylesheet" media="screen">
	</head>
	<body data-spy="scroll">		
		<div class="container">
			<div class="row">
				<div class="span12">
					<div class="navbar navbar-inverse" data-target=".navbar" style="position:fixed;margin:10px 0px auto 0px;width:940px;box-shadow:0px 0px 5px 0px rgba(150,150,150,0.8);z-index:999;">
						<div class="navbar-inner">
							<a class="brand" href="#">Bootstrap StepWizard</a>
							<ul class="nav">
								<li><a href="#Introduce">Introduce</a></li>
								<li><a href="#Download">Download</a></li>
								<li><a href="#Install">Install</a></li>
								<li><a href="#Usage">Usage</a></li>
								<li><a href="#JavaScript">JavaScript</a></li>
								<li><a href="#About">About</a></li>
								<li><a href="introcn.html">中文</a></li>
							</ul>
						</div>
					</div>
				</div>
			</div>
		</div>
		<div class="container" style="margin-top:60px;">
			<div class="row">
				<div class="span12">
					<div class="hero-unit">
						<h1>Bootstrap StepWizard</h1>
						<p>bootstrap_stepwizard is a StepWizard with bootstrap</p>
						<p>
							<a href="https://github.com/eastpiger/bootstrap_stepwizard" class="btn btn-primary btn-large">
							  Visit GitHub
							</a>							
							<a href="http://www.eastpiger.com" class="btn btn-primary btn-large">
							  Visit My Homepage
							</a>
						</p>
					</div>
					<h2 id="Introduce" style="padding-top:60px;">Introduce</h2>
					<p>Sometimes I want to use the tabs of bootstrap just like a step wizard . There used to be many project to do it such as Fuel UX and many others but difficult to use .</p>
					<p>Fortunately , Bootstrap_StepWizard is a new project within 3kb files to do it easily just like using Bootstrap_Tabs.js . like this :</p>
					<br/>
					<br/>
					<ul class="nav nav-stepwizard nav-stepwizard_unabled" id="myStepWizard_show">
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
					<br/>
					<br/>
					<div class="btn-group">
						<button class="btn" id="pre_show">Previous</button>
						<button class="btn" id="next_show">Next</button>
						<button class="btn" id="index_show">Index</button>
						<button class="btn" id="index_jump">jump to index 3</button>
					</div>
					<h2 id="Download" style="padding-top:60px;">Download</h2>
					<p>This project contains two major file : <em>bootstrap_stepwizard.js</em> and <em>bootstrap_stepwizard.css</em> . You can also use its packed edition : <em>bootstrap_stepwizard.min.js</em> and <em>bootstrap_stepwizard.min.css</em> .</p>
					<p>You can download the project via github : <a href="https://github.com/eastpiger/bootstrap_stepwizard">https://github.com/eastpiger/bootstrap_stepwizard</a></p>
					<h2 id="Install" style="padding-top:60px;">Install</h2>
					<p>This project has reliance on <em>bootstrap</em> and <em>Jquery</em> and you should install them firstly .</p>
					<p>To install <em>Bootstrap_StepWizard</em> , you should type this in your webpage :</p>
					<pre>
&lt;link href="bootstrap_stepwizard.css" rel="stylesheet" media="screen"&gt;
&lt;script src="bootstrap_stepwizard.js"&gt;&lt;/script&gt;</pre>
					<h2 id="Usage" style="padding-top:60px;">Usage</h2>
					<p>To show <em>Bootstrap_StepWizard</em> in your page , you can just type this in your webpage :</p>
					<pre>
&lt;ul class="nav nav-stepwizard" id="myStepWizard_show"&gt;
	&lt;li class="complete"&gt;&lt;span href="#home" data-toggle="tab"&gt;&lt;span class="badge"&gt;1&lt;/span&gt;Home&lt;/span&gt;&lt;/li&gt;
	&lt;li class="active"&gt;&lt;span href="#profile" data-toggle="tab"&gt;&lt;span class="badge"&gt;2&lt;/span&gt;Profile&lt;/span&gt;&lt;/li&gt;
	&lt;li&gt;&lt;span href="#messages" data-toggle="tab"&gt;&lt;span class="badge"&gt;3&lt;/span&gt;Messages&lt;/span&gt;&lt;/li&gt;
	&lt;li&gt;&lt;span href="#settings" data-toggle="tab"&gt;&lt;span class="badge"&gt;4&lt;/span&gt;Settings&lt;/span&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;div class="tab-content"&gt;
	&lt;div class="tab-pane active fade in" id="home"&gt;Home is a home.&lt;/div&gt;
	&lt;div class="tab-pane fade" id="profile"&gt;Profile can see the profile.&lt;/div&gt;
	&lt;div class="tab-pane fade" id="messages"&gt;Message allows you to send messages.&lt;/div&gt;
	&lt;div class="tab-pane fade" id="settings"&gt;Settings ... just as you know.&lt;/div&gt;
&lt;/div&gt;</pre>
					<p><strong>It is similer to use <em>bootstrap-tab.js</em> . Just replace <code>nav-tabs</code> into <code>nav-stepwizard</code> .</strong></p>
					<br/>
					<p>If you don't wnat users to click the button ( just like the example above ) , Just add a class <code>nav-stepwizard_unabled</code> .</p>
					<pre>
&lt;ul class="nav nav-stepwizard nav-stepwizard_unabled" id="myStepWizard_show"&gt;</pre>
					<h2 id="JavaScript" style="padding-top:60px;">JavaScript</h2>
					<p>This project alse contains some js functions . you can use them in js or Jquery .</p>
					<br/>
					<h4><em>stepwizard_prev function</em></h4>
					<pre>
function stepwizard_prev(handle)</pre>
					<p>example:</p>
					<pre>
$("#pre_show").click(function(){
	stepwizard_prev($("#myStepWizard_show"));
});	</pre>
					<p><strong>It returns -1 when the active tab is the first .</strong></p>
					<br/>
					<h4><em>stepwizard_next function</em></h4>
					<pre>
function stepwizard_next(handle)</pre>
					<p>example:</p>
					<pre>
$("#next_show").click(function(){
	stepwizard_next($("#myStepWizard_show"));
});</pre>
					<p><strong>It returns -1 when the active tab is the last .</strong></p>
					<br/>
					<h4><em>stepwizard_to function</em></h4>
					<pre>
function stepwizard_to(handle,index)</pre>
					<p>example:</p>
					<pre>
$("#index_jump").click(function(){
	stepwizard_to($("#myStepWizard_show"),3);
});</pre>
					<p><strong>It returns -1 when the target index is unabled .</strong></p>
					<br/>
					<h4><em>stepwizard_index function</em></h4>
					<pre>
function stepwizard_index(handle)</pre>
					<p>example:</p>
					<pre>
$("#index_show").click(function(){
	alert(stepwizard_index($("#myStepWizard_show")));
});</pre>
					<p><strong>It returns the active index .</strong></p>
					<h2 id="About" style="padding-top:60px;">About</h2>
					<p>Welcome to my homepage at <a href="http://www.eastpiger.com">www.eastpiger.com</a> .</p>
					<br/>
				</div>
			</div>
		</div>
			</div>
		</div>
		<script src="http://lib.sinaapp.com/js/jquery/2.0.3/jquery-2.0.3.min.js"></script>
		<script src="http://lib.sinaapp.com/js/bootstrap/2.3.2/js/bootstrap.min.js"></script>
		<script src="bootstrap_stepwizard.js"></script>
		<script type="text/javascript">
		$(function(){	
			$("#pre_show").click(function(){
				stepwizard_prev($("#myStepWizard_show"));
			});	
			$("#next_show").click(function(){
				stepwizard_next($("#myStepWizard_show"));
			});
			$("#index_show").click(function(){
				alert(stepwizard_index($("#myStepWizard_show")));
			});
			$("#index_jump").click(function(){
				stepwizard_to($("#myStepWizard_show"),3);
			});
		})
	</script>
	</body>
</html>