# Final Project Presentation Guide

这份指南旨在帮助大家准备 Final Project 的展示。根据 `README.md` 中的评分标准，你的展示应该涵盖以下关键部分，以确保能够展示出你们在各个 Level 中的工作成果。

## 项目概览 (Project Overview)

* **简要介绍**: 一句话概括你们构建的网络通信系统。
* **团队成员**: 列出小组成员及分工。

## Level 1: 点对点通信 (Point-to-Point Communication) - [30分]

*这部分重点展示基础通信链路的实现。TIPS: 你可以使用随机生成的1/0 binary序列来模拟上层比特流。*

- 录屏展示Level 1的完整的比特流传输过程。
- 录屏展示Level 1的消息分片传输功能。
- 展示在有噪声 (`noise_level > 0`) 情况下系统的表现。
- 观察不同噪声下的系统性能。
- 跟香农公式进行比较。(B log2(1+SNR)))

## Level 2: 多主机通信 (Multi-Host Communication) - [30分]

*这部分重点展示网络拓扑和交换/路由逻辑。*

- 录屏展示针对简单拓扑的多主机通信的完整过程。
- **寻址机制 (Addressing)**:
  - 你们如何区分不同的主机？
  - 数据包头 (Header) 是如何设计的？
- **路由与转发 (Routing & Forwarding)**:
  - 中心节点 (Switch/Router) 如何根据地址将消息转发给正确的目标主机？

## Level 3: 扩展功能 (Extension Features) - [最高 40分]

*选择你们实现的扩展功能进行详细介绍。需要基于Level 2完整实现。需要演示功能以及解释你们的实现方法。*

* **传输层 (Transport Layer)**: 可靠传输 (ACK/NACK)、序列号、超时重传、流控等。
* **信道编码 (Channel Coding)**: 纠错码、误码率 vs 纠错率的性能测试；有无信道编码的信息传输速率测试。
* **应用层协议 (Application Layer)**: 自定义协议设计 (HTTP/FTP-like)、请求-响应模式。需要基于你自己的 level 1/level 2 完整实现一个有实际意义的应用层协议。
* **性能优化 (Performance)**: 多种调制方式对比 (ASK/FSK/PSK)、抗噪性能分析。
* **无线通信 (Wireless)**: 无线信道模拟、MIMO、波束成形等。
* **并发处理 (Concurrency)**: 多线程处理、高并发访问支持。

## 遇到的挑战与解决方案 (Challenges & Solutions)

* 在开发过程中遇到了什么困难？
* 你们是如何解决这些问题的？
