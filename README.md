### 🔨基于zabbix-docker alpine镜像的Dockerfile做的一些更改

- 修改`PHP_TZ`以及系统默认时区为`Asia/Shanghai`(不然时间相差8小时)

- 修改默认Web字体为`微软雅黑`(不然显示不了中文)

- 添加`Python3`的支持(人生苦短，容器内用Python3执行脚本)

  #### 运行方法
  
  1. **build**
  
     ```shell
     docker build -t <imageName> .
     ```
  
  2. **run**
  
     ```shell
     docker run --name <containerName> -p 80:80 -p 10051:10051 -d <imageName>
     ```
  
     
  
  ***

<h1 style="text-align:center">LOVE♥Python,LOVE♥Docker </h1>
