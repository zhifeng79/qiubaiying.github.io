---
layout:     post
title:      How To Delivering Project On Time and On Value, as QA 
subtitle:   Tips and Strategies fro Better,Faster Testing 
date:       2018-12-31
title:      How To Delivering Project On Time and On Value, as QA 
author:     zhifeng.jiang
header-img: img/post-bg-BJJ.jpg
catalog: true
tags:
    - QA
    - Testing
---

> 参考  [《测试架构师修炼之道》](http://yuedu.163.com/book_reader/3d5f4dc163604ce48392b97430de6ed9_4)
> 参考 [《MFQ&PPDCS》] (http://hejiajie.cn/wp-content/uploads/2013/05/MFQPPDCS.pdf)


### 目录

- 测试团队职责
- 完成职责关键点
- 正确制定测试策略
- How to Test often
- 测试框架个人经验
- 性能测试
- 版本质量评估
- 测试闭环
- AI is coming


## 测试团队职责
 作为测试团队，完成项目各个版本各个功能各自类型的测试，尽力发现各类Bug，是不够的。设想一下如果版本晚上就要外发了，测试团队突然发现了一个严重的问题，问题影响外发，项目经理叫来开发紧急修改，搭上测试一通赶工，版本勉强赶上外发，或者推迟外发了，不是理想状态。
 测试团队应该在限定时间内尽早，尽快的发现各类问题。这就需要我们基于“产品质量目标”，基于“风险”，在充分考虑“产品研发状态”的前提下安排各类测试活动，在限定时间内进行刚刚好的测试。
 并且测试团队应该认识产品，确认产品功能是否满足客户需求，确认产品在非功能属性（性能，可靠性，易用性）的目标。
 在需求分析阶段预防缺陷。
 Testing is about reducing risk.

## 完成职责关键点
- 了解领域知识，客户需求，产品，业界规范，竞品
  例如手游加速的产品测试，需要了解热门手游Top10,2019年最值得期待的手游，手游分类，最耗流量手游Top 10,手游服务端架构设计，经典游戏服务器端架构概，全球同服手游解决方，游戏中的网络延迟，手游加速哪个好用， 手游性能测试
- 尽早测试
  测试的阶段：需求分析，UT，FT，ST，探索性，上线测试，特性交付于团队，灰度发布，蓝绿发布
- 尽快测试
  测试环境，测试人力，测试脚本，测试工具
- 正确的测试策略
- 正确评估产品质量；find the 'good enough' threshold
  问题影响，发生概率，发生频率，是否可规避，规避成本，情感影响
- 客户

## 正确制定测试策略
  Automation is good, but is doesnt fix poor test design
- 测试对象和范围是什么
- 测试的目标是什么
- 测试的重点和难点是什么
- 测试的广度和深度是什么
- 如何安排各种测试活动
- 如何评价测试的效果

### 了解产品的商业目标

- 产品亮点
- 产品竞争力
- 产品商业目标

### 梳理用户的使用场景
- 客户所在公司的组织架构
- 客户自身的职责
- 产品使用场景,使用习惯
- 同样的场景,竞品是否更有价值
- 客户分类后，抽象分析
- 综合考虑后出产品的拓扑模型，配置模型，流量模型

### 测试分层
- 尽可能的尽早测试
- 测试分层金字塔
[测试分层] (http://link.zhihu.com/?target=http%3A//wenku.baidu.com/link%3Furl%3DEQH46l7URJ14WqNNUe_QLhqfxy1O9HH6tDNqNMgq5Yyb8Bj8j5S02ElyE6OPMBP7MJ8p4he3-60bwRNizFnMfkTnJAI_VxagTUw4r1CcLi7)
- 算法测试 UT
- FT测试外围fake
- ST全真实系统

## How to Test Often Test Early
- Continuous_testing
- DevOPS

### CI,CD使得测试更加频繁
- 每次 commit
- 每次 merge
- 每小时
- 每天
- 每周
- 每个release

### 测试技术选型
- 站在别人的肩膀上
- 从多维度进行技术选型
  功能对比，兼容性对比，社区热度，社区成熟度，入门门槛， 二次开发的能力
- 够用就行

## 技术框架个人经验
- 基于领域关键字的测试框架
- 数据和逻辑分离
- 测试环境自动构建

### Web测试框架选型
- Seleium + robotframe
- 基于page obj的web测试框架
- Select web 控件的相对稳定

### CD 框架选型
- jenkins + ansible + repo
- ansible VS salt
- 多分支处理
- 资源动态调度

### 手机APP测试框架选型
- App云测试服务对比

### How to test AI Models
- Data Validation
- Core Algorithm ，Model validation，learnability, algorithm efficiency and empathy
- Feedback
- output is not fix

### How to test 算法
- Is it theoretically correct?
- Test with small dataset
- Test with large dateset


## 性能测试
- 满配置测试（用户模型抽象分析）
- 空跑base line
- 指标测试
  web 速度
- 并发数测试
- overload测试
- 观测指标
  cpu ,内存，磁盘IO， 网络IO， 磁盘占用
- 7*24测试

### 性能测试框架
- 全部自动化上线
- 框架locust
- 最小代价外围桩


### How AI will change the Tester
- AppDiff, a company that uses AI to test mobile apps.
- https://www.slideshare.net/practitest/testing-and-ai



