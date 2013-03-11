## Sumeru Todos Demo

## 一. 简介

在《Suemru MVC简介》中介绍如何在Suemru中添加model，使用了完整的MVC模式开发了“mvcTest”实例，在这篇文档中将更加深入将如何使用Suemru快速的开发一个webapp---“Todos”。

### 1. Todos Demo介绍

Todos Demo功能是记录用户需要完成的任务列表，当任务完成后可删除已经完成的任务。

#### 1.1 预览地址

<http://sumerudemo.duapp.com/debug.html#/todos>

#### 1. 2 预览图

![](images/todos_1_1.2.png)

### 2. Todos Demo作用

本文档以Todos Demo为例，介绍Sumeru Framework结构以及相关的语法，并重点介绍如何使用Suemru Framework开发webapp。

## 二. 如何使用Sumeru Framework开发Todos Demo

###1. 在model文件夹下添加todosModel.js和package.json

todosModel.js:


















package.json：

	suemru.packages{
	








在第二步的controller中subscribe方法中通过session.bind()方法将数据绑定到view指定的模块或者元素上，该模块或者元素内部可以使用handerbars语法来获取和使用数据（关于handerbars的语法请查看：<http://handlebarsjs.com>）。

todos.html

	<block tpl-id="todos">




### 5. 在assets/css/文件夹下编写todos.css 

todos.html完成后，需要使用css样式进行美化，详细的css的代码请查看：



![](images/todos_2_5.png)	

### 6.修改controller文件下的todosController.js 

修改controller文件夹下的todosController.js文件，在env.onready()方法中添加对view事件的监听和响应。 












添加后点击的效果图：


**6.4 controller中添加对单条数据选中和删除单条数据的事件响应**

	env.onready = function(){







	Sumeru.router.add(

 ![](images/todos_2_7.png)
 