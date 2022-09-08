# consul中文文档
一边学习一边翻译,希望自己能坚持下去
基于1.13x
## 开始使用
Consul的安装非常简单.有三种方法可以安装consul:
* [通过二进制文件](https://www.consul.io/docs/install#precompiled-binaries)
* [从源码编译安装](https://www.consul.io/docs/install#compiling-from-source)
* [在Kubernetes安装](https://www.consul.io/docs/k8s/installation/install)

下载二进制文件是最简单的方法,我们提供了基于TLS和SHA256验证的二进制文件.我们还分发PGP认证来验证SHA256结果
“开始使用”提供了在你本地机器上快速安装和使用的介绍

### 预先编译的文件
下载适合你系统的安装包来安装预先编译的文件,Consul目前被打包进一个zip文件.我们近期没有计划提供系统安装包

当zip包下载完成,解压到任意目录.运行consul不需要依赖其他任何文件

可以把二进制文件拷贝到任意地方.如果你想在命令行运行他,需要把它加入到系统路径

### 编译安装
编译安装需要安装go语言环境和git

可以从github上克隆代码

`
$ git clone https://github.com/hashicorp/consul.git \\
$ cd consul
`

编译安装后,二进制文件存放在./bin目录下

在本地系统中编译方法:
`make dev`

为其他系统编译方法(交叉编译):

通过下面的环境变量配置方法来指定目标系统
GOOS:目标系统类型,可选的有效值包含:linux, darwin, windows, solaris, freebsd
GOARCH:目标系统的架构,可选的有效值包含:386, amd64, arm, arm64

`
$ export GOOS=linux GOARCH=amd64 \\
$ make dev
`
### 浏览器兼容性
Consul目前支持所有的“长青树”浏览器.如果需要了解更多关于浏览器支持方面的信息,请访问[FAQ](https://www.consul.io/docs/troubleshoot/faq)

