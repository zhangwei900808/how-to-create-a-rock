# how-to-create-a-rock

## 1、什么是Luarocks？
Luarocks是一个Lua包管理器，基于Lua语言开发，提供一个命令行的方式来管理Lua包依赖、安装第三方Lua包等，社区比较流行的包管理器之一，另还有一个LuaDist，Luarocks的包数量比LuaDist多，更细节的两者对比可[参阅这里](http://notebook.kulchenko.com/zerobrane/lua-package-managers-luadist-luarocks-and-integration-with-zerobrane-studio)。

## 2、源码安装Luarocks

```
wget https://luarocks.org/releases/luarocks-2.4.1.tar.gz
tar -zxvf luarocks-2.4.1.tar.gz
cd luarocks-2.4.1
./configure
make build && make install
cd ..
```

## 3、创建.rockspec文件

```
mkdir lua-package
cd lua-package
luarocks write_rockspec
```

执行完之后会发现多了一个lua-package-dev-1.rockspec文件，这个文件就是我们创建的.rockspec文件，接着我们打开这个文件，查看里面的元信息，如下所示

```
#该包名
package = "lua-package"
#版本号(注意：1、版本号和你文件名所包含的版本号要一致，如这里的版本号是：dev-1，文件名是：lua-package-dev-1.rockspec
#2、版本号要以-x结尾，如0.0.1-1，1.3-1，如果你不按照这种规则定义则会报错！)
version = "dev-1"
source = {
   #指定源码的位置
   url = "*** please add URL for source tarball, zip or repository here ***"
}
description = {
   #该包所在的说明文档位置
   homepage = "*** please enter a project homepage ***",
   #指明所基于的开源协议
   license = "*** please specify a license ***"
}
build = {
   #编译方式
   type = "builtin",
   #指定包含的模块
   modules = {}
}
```
这里
## 

#
