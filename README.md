# how-to-create-a-rock

## 什么是Luarocks？
Luarocks是一个Lua包管理器，基于Lua语言开发，提供一个命令行的方式来管理Lua包依赖、安装第三方Lua包等，社区比较流行的包管理器之一，另还有一个LuaDist，Luarocks的包数量比LuaDist多，更细节的两者对比可参阅这里。

## 源码安装部署Luarocks

```
wget https://luarocks.org/releases/luarocks-2.4.1.tar.gz
tar -zxvf luarocks-2.4.1.tar.gz
cd luarocks-2.4.1
./configure
make build && make install
cd ..
```

## 创建.rockspec文件
环境安装好之后，

#

#
