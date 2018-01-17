# Scrapy

#### https://docs.scrapy.org/en/latest/

Scrapy爬虫框架

## 命令行操作

#### 创建项目

> scrapy startproject <项目名>

#### 创建spider

> scrapy genspider \<spider文件名> <要爬取的域名>

#### 执行scrapy

> 项目根目录下，scrapy crawl  \<spider文件名>

#### scrapy的shell环境

> 可用于命令行调试页面，scrapy shell \<url>

* response
* test = response.css('.test')

#### 保存数据

> scrapy crawl \<spider文件名(不需要加.py)> -o test.json
>
> scrapy crawl \<spider文件名(不需要加.py)> -o test.csv
>
> scrapy crawl \<spider文件名(不需要加.py)> -o test.jl

##### 远程保存

> scrapy crawl \<spider文件名(不需要加.py)> -o ftp://user:pass@ftp.example.com/path/test.csv

#### 错误检测

> scrapy check
>
> 可以故意写错语法查看效果

