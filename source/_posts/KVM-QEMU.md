---
title: KVM & QEMU
hidden: true
author: Supdrewin
---

### QEMU 简介

QEMU 是一个可以安装运行多种不同架构的模拟器, 由于是模拟器, 其运行速度会非常慢, 但是它可以使用其它虚拟机化引擎进行加速, 以获得与虚拟机相近的性能, 你甚至可以直通设备, 就像组装电脑一样, 可玩性很高.

系统模式的QEMU如: qemu-system-<arch>
用户模式如: qemu-<arch>

我们一般在 Linux 下使用 QEMU, 所以虚拟化引擎首选 KVM, 当然你也可以选择[其它的](# "如: Xen等"). 默认情况下 QEMU 使用 TCG.

### 什么是 KVM(Kernel Virtual Machine)

### 选择机器类型  -machine|-M
  
### DIY 你的 CPU  -cpu
  
### 分配机器内存大小 & 配置热拔插 -m
  
### 设备 -device
  
  
### 示例
1. https://github.com/supdrewin/vista-kvm
