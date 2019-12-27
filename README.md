# multi-storage-spring-boot-project

[![Build Status](https://travis-ci.org/SaharaG/multi-storage-spring-boot-project.svg?branch=master)](https://travis-ci.org/SaharaG/multi-storage-spring-boot-project)
[![codecov](https://codecov.io/gh/saharag/multi-storage-spring-boot-project/branch/master/graph/badge.svg)](https://codecov.io/gh/saharag/multi-storage-spring-boot-project)
![license](https://img.shields.io/github/license/saharag/multi-storage-spring-boot-project.svg)
![maven](https://img.shields.io/maven-central/v/com.github.sahara/multi-storage-spring-boot-starter.svg)

Aliyun(OSS)、QCloud(COS)、HuaweiCloud(OBS)、Qiniu(KODO)、Upyun(USS)、Local File System - Read and write remote files with
 Spring `Resource` interface, as easy as local access

* Aliyun(OSS)
    * [doc](https://help.aliyun.com/product/31815.html?spm=5176.7933691.1309819.8.48042a66sYQ3DG) 
    * [source](https://github.com/aliyun/aliyun-oss-java-sdk)

* QCloud(COS)
    * [doc](https://cloud.tencent.com/product/cos/document)
    * [source](https://github.com/tencentyun/cos-java-sdk-v5)

* HuaweiCloud(OBS)
    * [doc](https://support.huaweicloud.com/sdk-java-devg-obs/zh-cn_topic_0073679956.html) 
    * [source](https://github.com/huaweicloud/huaweicloud-sdk-java-obs)

* Qiniu(KODO)
    * [doc](https://developer.qiniu.com/kodo)
    * [source](https://github.com/qiniu/java-sdk)
    
* Upyun(USS)
    * [doc](https://help.upyun.com/docs/storage/)
    * [source](https://github.com/upyun/java-sdk)


## Getting Started

### Dependencies

* Java 8+
* Spring Boot 2.0.0+


## Building from Source

If you want to try out latest features , it can be easily built with the [maven wrapper](https://github.com/takari/maven-wrapper). 
Your JDK is 1.8 or above.

```
$ ./mvnw clean install
```

## Modules

There are some modules in this project, let's take a look at below overview:



### [multi-storage-spring-boot-parent](multi-storage-spring-boot-parent)

The main usage of `multi-storage-spring-boot-parent` is providing dependencies management for other modules.



### [multi-storage-spring-boot-autoconfigure](multi-storage-spring-boot-autoconfigure)

`multi-storage-spring-boot-autoconfigure` uses Spring Boot's `@EnableAutoConfiguration` which helps core components to be auto-configured. 
It reduces code, eliminates XML configuration. 



### [multi-storage-spring-boot-actuator](multi-storage-spring-boot-actuator)

`multi-storage-spring-boot-actuator` provides production-ready features.


### [multi-storage-spring-boot-starter](multi-storage-spring-boot-starter)

`multi-storage-spring-boot-starter` is a standard Spring Boot Starter, 
which contains [multi-storage-spring-boot-autoconfigure](multi-storage-spring-boot-autoconfigure) 
and [multi-storage-spring-boot-actuator](multi-storage-spring-boot-actuator). It will be imported into your application directly.



### [multi-storage-spring-boot-samples](multi-storage-spring-boot-samples)

The samples project includes:

- [Alibaba Cloud OSS Storage](multi-storage-spring-boot-samples/alicloud-storage-samples)
- [QCloud COS Storage](multi-storage-spring-boot-samples/qcloud-storage-samples)
- [QiNiu KODO Storage](multi-storage-spring-boot-samples/qiniu-storage-samples)
- [Huawei Cloud OBS Storage](multi-storage-spring-boot-samples/huaweicloud-storage-samples)
- [UpYun Storage](multi-storage-spring-boot-samples/upyun-storage-samples)
- [Local FileSystem Storage](multi-storage-spring-boot-samples/filesystem-storage-samples)

## Developing

If you want to update license with template license file , it can be easily built with the [maven wrapper](https
://github.com/takari/maven
-wrapper). 
Your JDK is 1.8 or above.

```
$ ./mvnw license:format -P license
```
