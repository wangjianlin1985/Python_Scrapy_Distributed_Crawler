# Python_Scrapy_Distributed_Crawler
Python基于Scrapy-Redis分布式爬虫设计毕业源码案例设计
## 开发环境：Python + Scrapy框架 + redis数据库
## 程序开发工具： PyCharm
  程序采用 python 开发的 Scrapy 框架来开发，使用 Xpath 技术对下载的网页进行提取解析，运用 Redis 数据库做分布式， 设计并实现了针对当当图书网的分布式爬虫程序，scrapy-redis是一个基于redis的scrapy组件，通过它可以快速实现简单分布式爬虫程序，该组件本质上提供了三大功能：
scheduler - 调度器
dupefilter - URL去重规则（被调度器使用）
pipeline   - 数据持久化

  Scrapy是一个比较好用的Python爬虫框架，你只需要编写几个组件就可以实现网页数据的爬取。但是当我们要爬取的页面非常多的时候，单个主机的处理能力就不能满足我们的需求了（无论是处理速度还是网络请求的并发数），这时候分布式爬虫的优势就显现出来。
  而Scrapy-Redis则是一个基于Redis的Scrapy分布式组件。它利用Redis对用于爬取的请求(Requests)进行存储和调度(Schedule)，并对爬取产生的项目(items)存储以供后续处理使用。scrapy-redi重写了scrapy一些比较关键的代码，将scrapy变成一个可以在多个主机上同时运行的分布式爬虫。

