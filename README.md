init 创建新项目或添加子模块(下列代码，不需要执行)
------------------------------------------------
    git submodule add git@github.com:sparrowzoo/tomcat.git                      tomcat
	git submodule add git@github.com:sparrowzoo/logback.git                     logback
	git submodule add git@github.com:sparrowzoo/incubator-druid.git             incubator-druid
	git submodule add git@github.com:sparrowzoo/open-source-integration.git     open-source-integration
	git submodule add git@github.com:sparrowzoo/commons-lang.git                commons-lang
	git submodule add git@github.com:sparrowzoo/commons-io.git                  commons-io
    git submodule add git@github.com:sparrowzoo/commons-codec.git               commons-codec
	git submodule add git@github.com:sparrowzoo/netty.git                       netty
	git submodule add git@github.com:sparrowzoo/elasticsearch.git               elasticsearch
	git submodule add git@github.com:sparrowzoo/spring-framework.git            spring-framework
	git submodule add git@github.com:sparrowzoo/jedis.git                       jedis
	git submodule add git@github.com:sparrowzoo/mybatis-3.git                   mybatis-3
	git submodule add git@github.com:sparrowzoo/incubator-dubbo.git             incubator-dubbo
	git submodule add git@github.com:sparrowzoo/dubbo-samples.git               dubbo-samples
	git submodule add git@github.com:sparrowzoo/etcd.git                        etcd
	git submodule add git@github.com:sparrowzoo/mybatis-spring.git              mybatis-spring
    git submodule add git@github.com:sparrowzoo/quartz.git                      quartz
    git submodule add git@github.com:sparrowzoo/disconf.git                     disconf
    git submodule add git@github.com:sparrowzoo/incubator-skywalking.git        incubator-skywalking
    git submodule add git@github.com:sparrowzoo/commons-fileupload.git commons-fileupload
    git submodule add git@github.com:sparrowzoo/elastic-job-lite.git elastic-job-lite
    git submodule add git@github.com:sparrowzoo/rocketmq.git rocketmq
    git submodule add git@github.com:sparrowzoo/zookeeper.git zookeeper
    git submodule add git@github.com:sparrowzoo/fastjson.git fastjson
    git submodule add git@github.com:sparrowzoo/druid.git druid
    git submodule add git@github.com:sparrowzoo/elastic-job-example.git elastic-job-example
    git submodule add git@github.com:sparrowzoo/redisson.git redisson
    git submodule add git@github.com:sparrowzoo/id-generator.git  id-generator
    git submodule add git@github.com:sparrowzoo/logback-extensions-spring.git logback-extensions-spring
    git submodule add git@github.com:sparrowzoo/incubator-skywalking-data-collect-protocol.git incubator-skywalking-data-collect-protocol
    
            	
客户端批量代码clone
---

初始化 
---

	git clone git@github.com:sparrowzoo/open-source-integration.git
	cd open-source-integration
	git submodule update --init
	git submodule foreach git checkout master
	
批量命令
----

	git submodule foreach git ...[fetch|pull|checkout...]


maven
---
mvn clean install -U -Dmaven.test.skip  -Dmaven.javadoc.skip=true