#### Yitian Huang
 - **Candidate Info**： 2-3 yeas in workforce | half year at this job | Male | 1990.11 |M.S| Computer Science
 - **Cell**：`+1-(703)-395-3877` | _Currently in North America, online or phone interview preferred._
 - **Email**：`wfgydbu@163.com` | **Wechat**：`wfgydbu`(2020)
 - **Blog**：[Ethan's Journal](https://journal.ethanshub.com/) | **Github**：[https://github.com/wfgydbu](https://github.com/wfgydbu)
 - **Position Expected**：Junior/Senior Python SE (Web Crawl/Backend) | **Location Expected**：Shanghai City

##### Education
- **The George Washington University** | 2015/09 - 2017/05 | Computer Science | M.S. | GPA：3.97/4.0 | Focus：OS, Network, Security, Database
- **Nanjing Tech University** | 2008/09 - 2012/06 | Computer Science and Technology | B.S.

##### Experience
- **Acuty LLC** | *Software Engineer (internship)* | 2017/10 - Now 
- **Tica Energy Data management Ltd** | *Software Engineer* | 2013/0 – 2014/04
- **Chinasoft International Ltd** | *Test Engineer* | 2012/03 - 2013/05

------

#### 部分项目经历
##### Python爬虫项目 | 所有代码均已上传到[Github](https://github.com/wfgydbu/PythonCrawlers) 
- **对`comic.kukudm.com`进行分布式全站爬取**
  - 使用`scrapy`和`scrapy_redis`框架，9个实例并行爬取（本机8个+云主机1个），每个实例16条并发，处理请求时峰值大约为27W/H；
  - 使用`pyspider`框架，单实例，15条并发，处理峰值大约为7W/H；
- **对`aqicn.org`进行分布式爬取**
  - 使用`celery`作为消息队列，2个实例，每个实例20条并发，大概160s完成一次所有监测点的爬取任务；
  - 构建定时任务定时爬取，绘制空气质量指数趋势图；
- **抓取`weibo.com`的关注页面和个人信息**
  - 模拟登陆新浪微博，获取Cookies；
  - 以登陆用户为种子，递归爬取每个用户的关注列表和个人信息页面；
  - 使用Bloom Filter和索引双重保障保证不会有重复的数据；
  - 预留接口便于扩展爬取其他页面；
- **抓取`taobao.com`某用户的历史订单**
  - 通过模拟用户输入账号密码和滑块拖动操作或通过扫描二维码登陆淘宝并获取Cookies；
  - 抓取用户所有历史订单；
- 其他
  - 验证码处理，一些常见图片处理或样本训练的算法实现。
  - 其他一些常见网站的爬取，包括`weather.com.cn`, `12306.cn`, `v.douyu.com`, `sougou.com`, `tieba.baidu.com`,   `xiami.com`, `music.163.com`, `toutiao.com`, `maoyan.com`, `qiushibaike.com`。

#####  Python项目 - ohHTMLToMarkdown库 | 代码已上传[Github](https://github.com/wfgydbu/ohHTML2Markdown) | 在PyPI搜索`ohHTMLToMarkdown`安装

- 一个HTML转Markdown的Python库，可以将一部分或整个HTML页面转化为Markdown文档。
- 利用bs4将HTML文档解析成块状结构，然后通过自定义方法对HTML标签进行处理：直接转化成md语义、进一步递归解析或直接舍弃。目前支持几乎所有主流HTML标签。转化效果基本满足需求，提供基本的测试代码，测试对象包括简书的文章、知乎的回答和我博客中发布过的文章。

##### Python项目 - ohIPPool代理IP池 | 代码已上传[Github](https://github.com/wfgydbu/ohIPPool)
- 一个基于Python、Redis和Flask的动态代理IP池。
- 提供配置项，可以轻易按需求调整配置并部署到服务器；通过接口或爬虫大量获得免费代理IP，使用Redis的有序集合对IP进行存储和管理，采用计分机制保证池中IP的质量，定期清理低质量或无效IP；对外开放一个Web接口服务，通过简单的GET请求就可以获得一个有效且高质量的代理IP。

##### 网站项目

- **类博客的内容展示网站**，Django框架 + Python开发，用于展示从`tieba.baidu.com`爬取到的内容，每个帖子对应网站中一篇文章。代码已上传[Github](https://github.com/wfgydbu/A-Django-Content-Site)。
- **TIME任务管理系统**，WordPress框架 + PHP开发，前端使用CSS、HTML和JavaScript，数据库使用MySQL，最终以插件形式发布。实现了一个面向个人的任务追踪管理系统，系统功能包括任务和项目进度追踪、统计报表生成（各种图、表）、数据导入导出等。代码已上传[Github](https://github.com/wfgydbu/timeistime) | [Demo](http://actionpeach.com/)

------

#### 工作期间项目

##### ESM能源管理系统 
**2013年7月 - 2014年4月 | 天加能源数据管理有限公司 | 10人开发团队 | 职位：软件工程师 |  部门：云计算中心 | 行业：互联网/能源 | 语言：C/C++, SQL**

- 实现一个能源管理系统，功能主要包括对定点能源消耗的实时监控和定期生成能源报告，报告交由能源专家进行分析以发掘节能潜力。
- 负责：
  - 设计和开发数据处理模块和DBA模块，前者按照自定协议接收来自工控设备的能源数据（水、电、温度湿度等），处理之后传输给DBA模块；后者在接受到数据后写入到数据库。

  - 部署并维护了一个MySQL集群（2主1备），前端部署负载均衡模块，对外提供数据服务。集群主要用来存储系统采集到的数据，同时向Web界面提供数据；

  - 设计并编写表结构、视图和存储过程的SQL脚本。


##### WISG-SCG产品线测试
**2012年3月 - 2013年5月 | 中软国际资源服务有限公司南京分公司 | 项目组约100人，属于10人测试小组 | 职位：测试工程师 |  部门：Consumer | 行业：通信 | 语言&工具：shell，自研测试工具**

- 外包到华为南研所移动宽带价值增长业务解决方案下的SCG项目组，项目主要为通信运营商提供第三方的计费及各类通信增值服务。 
- 负责：
  - 几个特定版本的计费功能测试：在实验环境(suse 11)下手动执行测试用例； 
  - 几个特定版本的自动化测试：使用华为自研的自动化测试工具执行和维护各版本自动化测试用例，维护各版本的自动化测试环境；
  - 负责几个特定版本的性能测试，部署镜像环境进行功能和性能测试。 支持海外工程师的局点项目部署。

------

#### 语言水平

**英语** CET-6 425|TOELF 92|留学经历

日常英语交流，擅长英语阅读和写作。《Adventures in Minecraft》中文译者之一，《Minecraft Modding For Kids For Dummies》和《Ruby for Kids For Dummies》独立中文译者，三本书均已由中国邮电出版社出版。

------

#### 自我描述
- 有较丰富的编程经验，熟悉多种编程语言，目前最擅长的语言是C和Python。
- 有扎实的计算机知识体系，热衷于操作系统、网络和安全领域。希望能够融汇贯通，学以致用。
- 很强的自学能力，能很快的上手之前没有接触过技术，遇到问题能迅速从互联网上定位到需要的信息并构建初步的解决方案。善于总结，博客上共计发布技术文章100余篇以及一部关于密码学入门的WIKI。
- 敏捷开发理念的追随者。

**技能点**（排名不分先后）：

- 常用Python库：
  - **爬虫相关**：scrapy, scrapy_redis, pyspider, celery, bloomfilter,  requests, bs4等
  - **图像处理**：tesserocr, numpy, PIL, matplotlib, cv2等
- **语言**：Python 3, C/C++, HTML5, CSS, JavaScript, PHP,  Shell
- **框架**：Django, Flask, WordPress
- **系统**：Windows, Linux, Amazon Web Service/EC2
- **数据库**：MySQL, MySQL Cluster, Oracle, SQLite, Redis

