# 在Linux上学C

## 怎么构建

切换到当前目录  
运行`docker build -t bluewaitor/linuxc:lastest -t bluewaitor/linuxc:0.0.1 .`  
发布`docker push bluewaitor/linuxc`  

## 如何运行

`docker run -it -v <C代码的绝对路径>:/code bluewaitor/linuxc`  
默认执行`gcc -v`打印出`gcc`的版本。  
可以使用`--entrypoint /bin/sh`覆盖原来`gcc`的命令。  
