基于Lucene的全文检索框架

一、	介绍

> 基于Lucene的全文检索框架，提供快速方便的索引创建及查询方式，并提供扩展功能对框架进行扩展。

二、	使用指南

1、	环境要求

> Java1.5+

> Lucene 3.0.x+

2、	加载

> 通过	RetrievalApplicationContext 载入配置参数，创建实例，每个被创建出的
> RetrievalApplicationContext实例中都包含一个完整的、独立的上下文环境。

> 一般情况下，一个应用只需要在启动时创建一个RetrievalApplicationContext实例，然后由整个应用共享。

3、	参数配置

> 默认配置文件为classpath下的retrieval.properties

4、	索引

4.1、初始化索引

4.2、提供5种方式创建索引

	以普通方式创建索引

	对单条数据库记录内容创建索引

	对单个文件内容及文件信息创建索引

	对数据库记录进行批量创建索引

	对大量的文件批量创建索引

	支持多线程创建索引，而不会出现索引文件异常

5、	查询

> 使用RQuery实例，通过传入构造好的QueryItem实例进行查询，并使用QuerySort实例对结果排序

6、	扩展

> 提供两种途径进行扩展：

  1. 在配置文件指定扩展类，在加载时，自动读取和设置配置文件中的扩展类

> 2）在RetrievalProperties实例中设置扩展类，并使用该实例创建RetrievalApplicationContext实例

7、	其它

> 更详细的示例请查阅test中的代码

> snoics-retrieval项目中使用了snoics-base.jar，如果需要获取snoics-base.jar的源代码，请到
> http://code.google.com/p/snoics-base/ 下载

三、	关于

> 项目地址：http://code.google.com/p/snoics-retrieval/

> Email : snoics@gmail.com

> Blog : http://blogjava.net/snoics

