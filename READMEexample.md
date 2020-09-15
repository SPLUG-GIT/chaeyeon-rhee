![pinpointlogo](https://github.com/naver/pinpoint/blob/master/web/psd/logo.png)

[![Build Status](https://travis-ci.org/naver/pinpoint.svg?branch=master)](https://travis-ci.org/naver/pinpoint)
[![codecov](https://codecov.io/gh/naver/pinpoint/branch/master/graph/badge.svg)](https://codecov.io/gh/naver/pinpoint)

**Visit [our official web site](www.naver.com) for more information and [Latest updates on Pinpoint](www.naver.com).**

## Latest Release (2020/09/09)
We're happy to announce the release of Pinpoint v2.1.0. Please check the release note at (https://github.com/naver/pinpoint/releases/tag/v2.1.0).

The current stable version is [v2.1.0](www.naver.com).

## Live Demo
Take a quick look at Pinpoint with our [demo](www.naver.com)!

## PHP, PYTHON
Pinpoint also supports application written in PHP, Python. [Check-out our agent repository](www.naver.com).

## About Pinpoint

**Pinpoint** is an APM (Application Performance Management) tool for large-scale distributed systems written in Java / PHP/PYTHON. Inspired by [Dapper](https://www.naver.com/), Pinpoint provides a solution to help analyze the overall structure of the system and how components within them are interconnected by tracing transactions across distributed applications.

You should definitely check **Pinpoint** out If you want to

* understand your [application topology](https://www.naver.com/) at a glance
* monitor your application in Real-Time
* gain code-level visibility to every transaction
* install APM Agents without changing a single line of code
* have minimal impact on the performance (approximately 3% increase in resource usage)

## Getting Started

* [Quick-start guide](https://www.naver.com/) for simple test run of Pinpoint
* [Installation guide](https://www.naver.com/) for further instructions.

## Overview

Services nowadays often consist of many different components, communicating amongst themselves as well as making API calls to external services. How each and every transaction gets executed is often left as a blackbox. Pinpoint traces transaction flows between these components and provides a clear view to identify problem areas and potential bottlenecks.
For a more intimate guide, please check out our [Introduction to Pinpoint video clip](https://www.naver.com/)

* **ServerMap** - Understand the topology of any distributed systems by visualizing how their components are interconnected. Clicking on a node reveals details about the component, such as its current status, and transaction count.

* **Realtime Active Thread Chart** - Monitor active threads inside applications in real-time.

* **Request/Response Scatter Chart** - Visualize request count and response patterns over time to identify potential problems. Transactions can be selected for additional detail by dragging over the chart.

![ex_screenshot](https://github.com/naver/pinpoint/blob/master/doc/images/ss_server-map.png)

* **CallStack** - Gain code-level visibility to every transaction in a distributed environment, identifying bottlenecks and points of failure in a single view.
![ex_screenshot](https://github.com/naver/pinpoint/blob/master/doc/images/ss_call-stack.png)

* **Inspector** - View additional details on the application such as CPU usage, Memory/Garbage Collection, TPS, and JVM arguments.
![ex_screenshot](https://github.com/naver/pinpoint/blob/master/doc/images/ss_inspector.png)

## Supported Modules

* JDK 6+
* [Tomcat 6/7/8/9, Jetty 8/9, JBoss EAP 6/7, Resin 4, Websphere 6/7/8, Vertx 3.3/3.4/3.5, Weblogic 10/11g/12c, Undertow](www.naver.com)
* Spring, Spring Boot (Embedded Tomcat, Jetty, Undertow), Spring asynchronous communication
* Apache HTTP Client 3.x/4.x, JDK HttpConnector, GoogleHttpClient, OkHttpClient, NingAsyncHttpClient, Akka-http, Apache CXF
* Thrift Client, Thrift Service, DUBBO PROVIDER, DUBBO CONSUMER, GRPC
* ActiveMQ, RabbitMQ, Kafka
* MySQL, Oracle, MSSQL(jtds), CUBRID, POSTGRESQL, MARIA
* Arcus, Memcached, Redis([Jedis, Lettuce](www.naver.com)), CASSANDRA, MongoDB, Hbase, Elasticsearch
* iBATIS, MyBatis
* DBCP, DBCP2, HIKARICP, DRUID
* gson, Jackson, Json Lib, Fastjson
* log4j, Logback, log4j2

## Compatability

Java version required to run Pinpoint:

|Pinpoint Version|Agent|Collector|Web|
|------|---|---|---|
|1.5.x|6-8|7-8|7-8|
|1.6.x|6-8|7-8|7-8|
|1.7.x|6-8|8|8|
|1.8.0|6-10|8|8|
|1.8.1+|6-11|8|8|
|2.0.x|6-13|8|8|
|2.1.x|6-14|8|8|

HBase compatibility table:
|Pinpoint Version|HBase 1.0.x|HBase 1.2.x|HBase 1.4.x|HBase 2.0.x|
|------|------|------|------|------|
|1.5.x|yes|nct tested|not tested|no|
|1.6.x|not tested|yes|yes|no|
|1.7.x|not tested|yes|yes|no|
|1.8.x|not tested|yes|yes|no|
|2.0.x|not tested|yes|yes|[optional](www.naver.com)|
|2.1.x|not tested|yes|yes|[optional](www.naver.com)|

Agent - Collector compatibility table:

|Pinpoint Version|Collector 1.5.x|Collector 1.6.x|Collector 1.7.x|Collector 1.8.x|Collector 2.0.x|Collector 2.1.x|
|------|------|------|------|------|------|------|
|1.5.x|yes|yes|yes|yes|yes|yes|
|1.6.x|not tested|yes|yes|yes|yes|yes|
|1.7.x|no|no|yes|yes|yes|yes|
|1.8.x|no|no|no|no|yes|yes|
|2.0.x|no|no|no|no|no|yes|
|2.1.x|no|no|no|no|no|no|

Flink compatibility table:
|Pinpoint Version|flink 1.3.x|flink 1.4.x|flink 1.5.x|flink 1.6.x|flink 1.7.x|
|------|------|------|------|------|------|
1.7.x|yes|yes|no|no|no|
1.8.x|yes|yes|no|no|no|
2.0.x|yes|yes|yes|yes|yes|
2.1.x|yes|yes|yes|yes|yes|

## Community

[Github issues](www.naver.com)
[Google group](www.naver.com)
[Gitter](www.naver.com)

We have Chinese community now, welcome to join!
|QQ Group1: 897594820|QQ Group2: 812507584|DING Group|
|---------------------|---------------------|---------------------|
![qrcode](https://github.com/naver/pinpoint/blob/master/doc/images/NAVERPinpoint.png)|![qrcode](https://github.com/naver/pinpoint/blob/master/doc/images/NAVERPinpoint2.png)|![qrcode](https://github.com/naver/pinpoint/blob/master/doc/images/NaverPinpoint%E4%BA%A4%E6%B5%81%E7%BE%A4-DING.jpg)

## License
Pinpoint is licensed under the Apache License, Version 2.0. See [LICENSE](www.naver.com) for full license text.

```
Copyright 2018 NAVER Corp.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

