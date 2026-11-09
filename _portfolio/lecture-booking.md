---
title: 学术讲座管理与预约系统
layout: project
permalink: /projects/lecture-booking/
order: 1
kind: Java 后端开发
period: 2025.10–2026.06
summary: 面向高校讲座场景，开发管理与预约接口，处理高并发预约中的超额与重复提交问题。
stack: [Java, Spring Boot, MyBatis-Plus, SQL]
---

## 后端接口

基于 Spring Boot 和 MyBatis-Plus 搭建后端服务架构，独立开发管理员端与用户端共 **8 个核心功能模块**的接口，覆盖权限管控、讲座发布、在线预约和数据统计。

## 数据建模与并发控制

梳理用户、讲座、预约、收藏等 **8 类业务实体**并设计数据表。对预约写入采用数据库事务和乐观锁，应对并发请求下名额超额与重复预约的问题。

![讲座预约流程示意图：提交请求、校验名额、通过事务和乐观锁写入预约记录]({{ '/images/booking-flow.svg' | relative_url }})

## 测试与性能

设计功能、性能和安全测试用例。通过优化 SQL 查询和建立索引，将项目测试中的核心接口平均响应时间控制在 **500 ms 以内**。配套开发管理端的数据可视化模块，支持运营统计。
