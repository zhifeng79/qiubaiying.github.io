---
layout:     slide
title:      How To Delivering Project On Time and On Value, as QA
description: A presentation slide for QA
theme: black
transition: slide
---

<section data-markdown>
# 目录
- 测试团队职责
- 完成职责关键点
- 正确制定测试策略
- 如何频繁的尽早的测试
- 测试框架个人经验
- 性能测试
- 版本质量评估
- 测试闭环
- AI is coming
</section>

<section data-markdown>
# 测试团队职责
- Find the Bug in Project
- On Time
- As Early as possible
- On Value
</section>

<section data-markdown>
# 测试团队职责
- 基于“产品质量目标”
- 基于“风险”
- 在充分考虑“产品研发状态”的前提下
- 安排各类测试活动
- 在限定时间内进行刚刚好的测试
- Testing is about reducing risk
</section>

<section data-markdown>
## 如何完成职责
- 了解领域知识，客户需求，产品，业界规范，竞品
- 尽早测试
- 尽快测试
- 正确的测试策略
- 正确评估产品质量
</section>

<section data-markdown>
## 正确制定测试策略
  Automation is good, but is doesnt fix poor test design
- 测试对象和范围是什么
- 测试的目标是什么
- 测试的重点和难点是什么
- 测试的广度和深度是什么
- 如何安排各种测试活动
- 如何评价测试的效果
  dashboard显示结果，信息可公开透明，可追溯； 产品导览指导众测和用户体验测试
</section>

<section data-markdown>
###测试对象和范围
- 产品做什么的
- 产品外部接口
- 产品什么组成
- 产品处理什么数据
- 产品怎么被使用
- 产品依赖的东西
- 产品和时间的相关方面
- XX性需求的要求
</section>

<section data-markdown>
### 四步测试策略制定法
- 明确产品质量目标
- 进行风险分析
- 适配产品发开发流程
- 测试分层
</section>

<section data-markdown>
 ### 领域知识
![领域知识](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/DomainKnowledge.jpg)
</section>

<section data-markdown>
### 了解产品的商业目标
- 产品亮点
- 产品竞争力
- 产品商业目标
</section>

<section data-markdown>
### 梳理用户的使用场景
- 客户所在公司的组织架构
- 客户自身的职责
- 产品使用场景,使用习惯
- 同样的场景,竞品是否更有价值
- 客户分类后，抽象分析
- 综合考虑后出产品的拓扑模型，配置模型
</section>

<section data-markdown>
### 需求测试分层
- 端到端的全真实环境自动化过度投入，把时间都浪费在维护不稳定的用例上
- 把容易出错的接口隔离，mock,fake,可以控制接口之间的交互，确保良好的测试覆盖率
</section>

<section data-markdown>
### google测试分层
- 小型测试
  SWE，独立功能模型，数据损坏，错误条件
- 中型测试
  SET SWE，功能邻进区
- 大型测试
  TS SET SWE 真实用户场景
</section>

<section data-markdown>
### 测试资源分层原则
![资源分层原则](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/google_test1.png)
</section>

<section data-markdown>
### 不同层次时间要求
- 小型  10ms 1分钟强制结束
- 中型  1s以内 5分钟强制结束
- 大型  尽可能快  15分钟强制结束
- 超大型 尽可能快  1小时
</section>

<section data-markdown>
### 不同层次的占比
- 小型 70%
- 中型 20%
- 大型 10%
</section>

<section data-markdown>
### 自动化用例原则
- 每个测试相互独立，任意执行，便于后期分拆，并发
- 每个用户做到测试环境还原
- 不要用sleep
- 自动化获取系统日志
</section>

<section data-markdown>
## 如何频繁的尽早的测试
- Continuous_testing
- DevOPS
</section>

<section data-markdown>
### CI,CD使得测试更加频繁
- 每次 commit
- 每次 merge
- 每小时
- 每天
- 每周
- 每个release
</section>

<section data-markdown>
### 如何减短自动用例执行时间
- 按照代码构建影响精确化测试范围，建立构建依赖示例图
- 测试资源池，并发测试
</section>

<section data-markdown>
### 测试技术选型
- 站在别人的肩膀上
  自动化投入的越多，维护成本也就越大
- 从多维度进行技术选型
  功能对比，兼容性对比，社区热度，社区成熟度，入门门槛， 二次开发的能力
- 够用就行
</section>

<section data-markdown>
## 技术框架个人经验
- 基于领域关键字的测试框架
- 数据和逻辑分离
- 测试环境自动构建
- 测试不做数据持久化
</section>

<section data-markdown>
### Web测试框架选型
- Seleium + robot
- 基于page obj的web测试框架
- Select web 控件的相对稳定
</section>

<section data-markdown>
### CD 框架选型
- jenkins + ansible + repo
- ansible, salt
- 多分支处理
- 资源动态调度
</section>

<section data-markdown>
### How to test 算法
- Is it theoretically correct?
- Test with small dataset
- Test with large dateset
</section>

<section data-markdown>
### 探索性测试方法 
![产品特性分区](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/exploreTest.jpg)
</section>

<section data-markdown>
### 历史区测试法
![历史区测试法](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/historyAreaTest.jpg)
</section>

<section data-markdown>
### 商业区测试法
![商业区测试法](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/BussinessArea.jpg)
</section>

<section data-markdown>
### 娱乐区测试法
![娱乐区测试法](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/entertainmentArea.jpg)
</section>

<section data-markdown>
### 破旧区测试法
![破旧区测试法](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/problemArea.jpg)
</section>

<section data-markdown>
### 手机APP测试框架选型
- App云测试服务
</section>

<section data-markdown>
### How to test AI Models
- Data Validation
- Core Algorithm ，Model validation，learnability, algorithm efficiency
- Feedback
- output is not fix
</section>

<section data-markdown>
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
</section>

<section data-markdown>
### 性能测试框架
- 全部自动化上线
- 框架locust
- 最小代价外围桩
</section>

<section data-markdown>
## 版本质量评估
- 是否常用主功能
- 问题影响
- 发生概率
- 是否可规避，规避成本
- 情感影响
- 是否容易诊断
- 让开发，产品经理，售后加入评估
- 要充当版本质量达标的推手
</section>

<section data-markdown>
## 测试闭环
![测试闭环](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/test_circle1.png)
</section>

<section data-markdown>
## How AI will change the Tester
- AppDiff, a company that uses AI to test mobile apps.
- https://www.slideshare.net/practitest/testing-and-ai
</section>

<section data-markdown>
## 测试闭环AI版本
![测试闭环AI版本](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/test_circle_ai.png)  
</section>

<section data-markdown>
 ### 测试AI从哪里学习
![测试AI从哪里学习](https://raw.githubusercontent.com/zhifeng79/zhifeng79.github.io/master/img/Test_Ai_Learn_from.png)  
</section>





































