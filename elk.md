## What are logs?
-logs--->records of events/status/transactions?
     --->What happened? Was there something wrong or all good?

## 集中式日志系统：
### 问题： 
   把分散在n个机器/设备/地点中的日志都收集起来，集中放在一个地方。同一个系统的不同app/component部署在了不同的vm上。
### 主要特点：
  > * 收集——能够收集多种来源的日志数据
  > * 传输——能够稳定的把日志数据传输到中央系统
  > * 存储——如何存储日志数据
  > * 分析——可以支持UI分析
  > * 警告——能够提供错误报告，监控机制

### 主要产品
- Rsyslog
- Syslog-ng
- Splunk(Commercial)
- Scribe(Facebook)
- Chukwa(Linkedin)
- Fluentd(Cloudera)
- ELK(Open source, Elastic.co)

## What is ELK Stack?
**E** ：Elasticsearch--a search and analytics engine.
        - open-source
        - distributed
        - RESTful （接口友好）
        - JSON-based 
        - scalable
        - easy to use
        - based on Apache Lucene
        - written in Java
        
**L** ：Logstash--
a server-side data processing pipeline that ingests data from multiple sources simultaneously, transform it, and then sends it to a "stash" like Elasticsearch.
        components:
        - Shipper 发送日志数据
        - Broker  收集数据，Redis by default
        - Indexer 数据写入
 
 [img](/logstashComponents.png)
        - 
**k** ：Kibana--lets users visualize data with charts and graphs in Elasticsearch
        - written in JS
        - frontend visualization
        - use Elasticsearch and interactive with data 
        

![img](/elk.png)
![img](https://jacaranda2016.github.io/webwxgetmsgimg.jpg)

![img](/ELK.jpg)

## How to install ELK?
Besides Elasticsearch, Logstash and Kibana, Nginx, Logstash-forwarder and JDK are also needed to be installed. 

[Install Instructions](https://www.ibm.com/developerworks/cn/opensource/os-cn-elk/index.html)

  
  
 
