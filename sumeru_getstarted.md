## 从这里开始




我们的sumeru是基于node.js运行，如果你的电脑已经安装了node.js环境，那么你可以使用下面命令很方便的安装sumeru。

我们先使用npm安装sumeru包：

	npm install -g sumeru
	
当sumeru包安装完成后，我们就可以使用sumeru开发自己的应用啦！在这之前我们需要先创建一个存放应用的文件夹，命令如下：

	sumeru init ./myproject
	
其实，当应用文件夹创建完成，一个基于sumeru的简单应用就诞生了，让我们先来看看他长什么样！

	cd myproject
	
	cd server
	
	node run.js
	
打开浏览器，在地址栏中输入 “localhost:8080/debug.html” 就可以看到咯！



#### 1.2 直接下载

当然，如果你觉得使用命令安装不符合你的风格，我们也提供直接下载sumeru目录的方式来生成应用目录，如果这是你想要的[请猛击这里](http://baidu.com)








	通过以上代码我们先添加一个router建立URl中hash部分与Controller之间的关系，关于router的具体用法我们会在后面的文档中做详细的说明，然后创建具体的controller。
	
		App.helloworld = sumeru.controller.create(function(env,session){


	











恭喜你已经完成了基于sumeru开发的第一个应用“Hello World”，来让我们来看看他是什么样的？

在浏览器中输入“localhost:8080/debug.html#/helloworld”,是否跟我的一样呢？

![](images/intro_2_1.png)
	 