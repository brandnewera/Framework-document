## Sumeru framework入门文档






























（2）在view文件夹下创建helloworld.html文件，文件内容如下：





Framework是基于node.js开发的，所以需要node.js环境以及需要数据库的支持，百度开发者中心上BAE提供整套的环境的支持，只需简单的配置就可以快速运行基于framework开发的应用，具体方法如下：







![](images/intro_4_4.png)

![](images/intro_4_5.png)

  	  - url : ^/socket/(.*)
    	script: $1.nodejs
    
      - url : ^/view/(.*)
        script: /__bae__/bin/view/$1
   
      - url : ^/bin/(.*)
        script: /__bae__/bin/$1

      - url : ^/static/(.*)
        script: /__bae__/static/$1 
        
      - url : ^/publish/(.*)
        script: /index.html 
    
      - url : /server/(.*)
        script: /index.html 

      - url : (*.ico)
        script: $1    
    
      - url : (*.html)
        script: $1

      - expire : .jpg modify 10 years
      - expire : .swf modify 10 years
      - expire : .png modify 10 years
      - expire : .gif modify 10 years
      - expire : .JPG modify 10 years
      - expire : .ico modify 10 years







![](images/intro_4_13.png)





































