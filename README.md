# distributedFileSystem

#### 介绍
在Linux环境下基于FastDFS实现的分布式文件系统服务器，QT开发跨平台客户端，可为用户或网站提供远程资源存
储服务。

#### 软件架构
C、Qt、FastDFS、Nginx、Redis、FastCGI、MySQL、Json

#### 完成的功能

- 使用安装FastDFS插件的Nginx代理解析HTTP请求，使客户端可以直接与存储节点进行通信，实现资源的快速下载与上传；
- 通过编写FastCGI接口解析客户端发送的具体请求信息，实现注册、登录、上传、下载等核心功能；
- 在客户端中构造URL和HTTP请求信息，发送HTTP请求对文件系统服务器进行交互；
- 使用生产者-消费者模型上传用户选定的文件。
