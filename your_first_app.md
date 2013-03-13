
#Your First App

sumeru是以Javascript为唯一开发语言并专注于开发移动App的云端统一开发框架，使用sumeru开发的App，既可以作为Web App运行，也可以打包作为Native App安装，其以打造全新App架构为使命，提供使用Javascript抹平云和端的新世界，你将不再需要切换语言分别编写服务器和客户端逻辑；你将不再需要花费原来50%以上的精力遍历、操作DOM和管理链接，只需专心编写最核心的业务逻辑。

在《从这里开始》中介绍了如何使用sumeru开发“hello world”，现在我们真正使用sumeru开发一个App。


### 首先预览一下这个App

![](images/firstapp.png)


###（1）在"app/model/"下创建firstApp.js，输入以下代码：

* firstApp.js

		Model.firstApp = function(exports){
	
		






###（3）在"app/publish/"下创建firstApp.js，输入以下代码

* firstApp.js









	大家发现了这里的controller与《从这里开始》中的controller不一样，多了"env.onload()"和"env.onready()"方法，关于controller后续将做专门的说明。








至此，App代码部分已经完成，在浏览器中输入"localhost:8080/debug.html#/firstapp"运行App。
	