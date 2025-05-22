# Undefined OS 项目文档

欢迎来到Undefined OS 项目文档。文档将介绍OS的总体架构设计，具体的实现内容，开发经历，以及与trust-os的比较。

## 项目介绍

项目主体是基于ArceOS和StarryNext编写的，对StarryNext的架构进行了较大的修改，修正和完善了ArceOS中的部分实现。在此基础上，我们实现了一百余个POSIX系统调用，提供了Linux兼容性，能够运行busybox等为Linux编译的实用程序。

## 项目特色

- 安全：使用Rust语言编写，提供了内存安全性，支持多CPU核心下的线程安全。
- 跨平台：支持x86_64/riscv64/aarch64/loongarch64 等多种指令架构，可以运行在qemu虚拟机和其他硬件开发板上。
- 兼容性：我们提供了兼容Linux的系统调用实现，同时保留了未来兼容其他OS的系统调用的接口。
