### 2020-04-17 Update for Python3
更新了适应python3的包，修改了一些运行上的错误。

### 安装步骤

- 创建python3虚拟环境：
```
virtualenv -p python3.x venv  
```
- 激活虚拟环境
```
source venv/bin/activate
```
- 安装Blog_mini需求文件
```
pip install -i http://pypi.douban.com/simple/ --trusted-host pypi.douban.com -r requirements/common.txt
```
- 使用sqlite作为默认数据库来运行Blog_mini
```
python manage.py deploy product
```
- 生成虚拟数据（可选）
```
python manage.py deploy test_data
```
- 运行
```
gunicorn manage:app
```
- 指定IP、端口运行
```
gunicorn -b 0.0.0.0:80  manage:app
```

---
==
---

### 资料整合

**0.功能详解文档**

​    功能详解：[《开源分享：用Python开发的开源博客系统Blog_mini》](http://xpleaf.blog.51cto.com/9315560/1748913)



**1.完整部署文档**

​    在CentOS上部署Blog_mini：[《在CentOS上部署开源博客系统Blog_mini》](http://xpleaf.blog.51cto.com/9315560/1748629)

​    在Ubuntu上部署Blog_mini：[《在Ubuntu上部署开源博客系统Blog_mini》](http://xpleaf.blog.51cto.com/9315560/1748707)



**2.完整数据库安装文档**

​    ***部署Blog_mini可以配置数据库，也可以完全不用配置数据库！**如果需要配置MySQL数据库，作者也撰写了详细完整的**MySQL安装**与**配置**以及**优化**的文档：

​    在CentOS上源码安装MySQL：[《在CentOS上源码安装MySQL+安装问题解决+安全优化 》](http://xpleaf.blog.51cto.com/9315560/1748063)    

​    在CentOS上yum安装MySQL：[《在CentOS上使用yum安装MySQL+安全优化》](http://xpleaf.blog.51cto.com/9315560/1748625)

​    在Ubuntu上源码安装MySQL：[《在Ubuntu上源码安装MySQL+安装问题解决+安全优化》](http://xpleaf.blog.51cto.com/9315560/1748824)

​    在Ubuntu上apt安装MySQL：[《在Ubuntu上使用apt-get安装MySQL+安全优化》](http://xpleaf.blog.51cto.com/9315560/1748704)

====
---

### 2018-07-06说明

之前的服务器地址140.143.205.19已经不可用，现已经更改为如下地址：

```
试用地址：http://122.152.231.228:8080/
帐号：blog_mini@163.com
密码：blog_mini
```

Blog_mini的Demo网站停了近一个月，由于6月份，几乎整个月的时间都忙于毕业的事情，也没有时间去处理，后段时间由于又给自己放了一个小假期，所以是迟迟未能解决问题，给部分想参考Demo的朋友带来不便，实在是非常抱歉！

现已经购买了一年的服务器时长，所以服务会一直运行下去，感谢大家的关注和支持！

### 2018-02-09说明

之前的服务器地址115.159.72.250已经不可用，现已经更改为如下地址：

```shell
试用地址：140.143.205.19
帐号：blog_mini@163.com
密码：blog_mini
```

承蒙大家喜爱，Blog_mini已经走过两年的时间了，从`star`和`fork`来看，很开心很高兴很多网友朋友能够把它作为自己入门Python和Python Web的一个小项目来进行学习，也正因为如此，一种不可言喻的责任就背负在身上，我总是担心这个小项目中可能出现的不可预知的坑会给部分初学的朋友带来很大的困难。大概从2017年开始，我就有意要整体改进和完善Blog_mini这个小项目。

然而过去两年作为大学阶段十分重要的两年，确实有太多的事情，因此这个计划一直耽误至今。眼看马上临近毕业，毕业设计也需要花费一定的时间和精力，所以还会继续耽误一小段时间。但不管如何，今年一定会努力争取完成这件事情。

计划将会从界面UI、后台管理系统、开发文档、代码注释等方面对这个小项目进行完善，这样之后，真心希望初学者都能够通过这样一个小项目来加强对Python基础技能以及其它技能的学习，达到可以使用Python进行基本开发这样的一种状态，去体验Python给自己带来的快乐。

---

# Blog_mini

### 1.功能强大的开源博客系统
Blog_mini是一个开源的博客系统，用Python开发完成，具有简洁的界面和强大的后台管理，

使用它，你可以轻松架设属于您自己的个人博客网站！

    只要把Blog_mini部署上，您不需要再进行任何命令上的操作即可以轻松使用和管理您的个人博客！

### 2.完整而详尽的部署文档
我们撰写了非常详细的部署文档，涵盖了CentOS和Ubuntu，可见下面地址：

    Blog_mini详细部署文档：http://xpleaf.blog.51cto.com/blog/9315560/1748871

作者亲测，在网络环境良好的情况下，最快用3分钟即可以把Blog_mini部署并上线！

### 3.提供试用地址
如果你只是想试用Blog_mini的功能，我们提供了试用地址：

    试用地址：115.159.72.250:8080
    帐号：blog_mini@163.com
    密码：blog_mini

已经有很多网友对Blog_mini进行了体验，我们欢迎您使用，并且能就使用过程中的一些问题给予作者意见和建议。

### 4.值得一学的源代码
如果你初学Python Web，或者你从来没有进行过一个完整项目的开发，或者你以后想从事Python自动化运维开发的工作，

不妨阅读并学习一下Blog_mini的源代码。

    Blog_mini采用结构清晰的工厂模式来设计开发，其中的一些开发思想模仿了国外牛人miguelgrinberg，因此，值得一学！

### 5.技术支持
如果你在部署和使用过程中有疑问，请给作者留言：

    作者51cto博客：http://xpleaf.blog.51cto.com
    作者个人博客网站：http://www.xpleaf.cn(目前不可访问)
    郑重说明：http://www.xpleaf.com这个域名已经被抢注，并且被用于发布不良内容，我将会进行举报！

