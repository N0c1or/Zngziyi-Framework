# Zngziyi Framework - GUI免杀生成工具

![Rust](https://img.shields.io/badge/Built_with-Rust-orange?logo=rust)
![GUI](https://img.shields.io/badge/Interface-GUI-blue?logo=windows-terminal)
![AntiVirus](https://img.shields.io/badge/Protection-免杀-success)

## 📜 框架概述

Zngziyi 是一款基于Rust语言开发的高级免杀载荷生成框架，专为红队行动和渗透测试设计。

## 🚀 核心特性

### 🔧 载体类型

- **Shellcode一体**
  内联式载荷，适用于快速部署场景
- **Shellcode分离**
  配置文件外部分离，增强隐蔽性
- **白加黑DLL**
  利用合法签名DLL实现隐蔽加载

### 🔐 加密方案

| 加密方式 | 密钥长度 | 特点                     |
| -------- | -------- | ------------------------ |
| RC4      | 动态可变 | 流式加密，高效快速       |
| XOR      | 256位    | 轻量级混淆，低开销       |
| AES-CFB  | 128/256  | 军用级安全，抗分析能力强 |

### 🕵️ 混淆技术

1. **UUID混淆**
  利用UUID编码混淆加密后的shellcode

2. **word混淆**
   利用大量单词混淆加密后的shellcode

### ⚡ 加载引擎

1. **直接加载**
   `ZwAllocateVirtual` 经典模式
2. **回调函数加载**
   利用系统回调机制实现无痕注入
3. **APC注入**
   异步过程调用实现进程注入
4. **白加黑APC**
   结合合法进程的增强型注入

### 🛡️ 反逆向手段

- **反调试系统**

- **反沙盒检测**

- **反虚拟机**

  
