# consul中文文档
一边学习一边翻译,希望自己能坚持下去
基于1.13x
## 开始使用
Installing Consul is simple. There are three approaches to installing Consul:
Consul的安装非常简单.有三种方法可以安装consul:
* [通过二进制文件](https://www.consul.io/docs/install#precompiled-binaries)
* [从源码编译安装](https://www.consul.io/docs/install#compiling-from-source)
* [在Kubernetes安装](https://www.consul.io/docs/k8s/installation/install)

下载二进制文件是最简单的方法,我们提供了基于TLS和SHA256验证的二进制文件.我们还分发PGP认证来验证SHA256结果
“开始使用”提供了在你本地机器上快速安装和使用的介绍

预先编译的文件
Precompiled Binaries
下载适合你系统的安装包来安装预先编译的文件,Consul目前被打包进一个zip文件.我们近期没有计划提供系统安装包

当zip包下载完成,解压到任意目录.运行consul不需要依赖其他任何文件

可以把二进制文件拷贝到任意地方.如果你想在命令行运行他,需要把它加入到系统路径

编译安装
编译安装需要安装go语言环境和git

可以从github上克隆代码

\` $ git clone https://github.com/hashicorp/consul.git
\`$ cd consul
