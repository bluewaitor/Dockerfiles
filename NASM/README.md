# 我的NASM

## 目的
为了学习`Assembly`，环境的问题很烦，所以创建这个镜像。

## 怎么构建
切换到当前目录  
运行`docker build -t bluewaitor/nasm:lastest -t bluewaitor/nasm:0.0.2 .`  
发布`docker push bluewaitor/nasm`  

## 如何运行
`docker run -it -v <汇编代码的绝对路径>:/code bluewaitor/nasm`  
默认执行`nasm -h`打印出`nasm`的帮助信息，可以在命令的后面使用`-v`重写`-h`打印版本。  
可以使用`--entrypoint /bin/sh`覆盖原来`nasm`的命令
