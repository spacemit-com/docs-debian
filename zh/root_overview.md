---
sidebar_position: 1
---

# 简介

**Debian** 是由社区维护的 Linux 发行版。进迭时空（SpacemiT）为 K1 和 K3 平台的部分设备提供 Debian 镜像，可用于日常办公、软件开发和设备调试。系统使用标准的 `.deb` 软件包格式，通过 APT 安装和更新软件。

## 系统架构

| 层级 | 说明 |
| --- | --- |
| 应用与桌面环境 | 提供图形桌面、系统工具和应用程序。 |
| Debian 用户空间 | 提供系统服务、应用框架、运行时和基础库。 |
| Linux 内核 | 管理进程、内存、文件系统和硬件设备。 |
| 底层固件 | 包含 SPL、OpenSBI 和 UEFI，负责早期硬件初始化、提供 RISC-V SBI 接口和引导操作系统。 |

## 软件组件

### 应用

- GNOME 桌面及其常用应用
- Chromium 浏览器
- LibreOffice
- Evince
- Loupe
- mpv
- Snapshot

### 框架

#### 应用框架

- GTK
- Qt

#### 多媒体框架

- FFmpeg (支持硬件加速)
- GStreamer (支持硬件加速)
- PipeWire
- MPP (进迭时空多媒体处理平台，提供 C API 和示例)

#### AI推理框架

- spacemit-onnxruntime
- llama.cpp-tools-spacemit

### 运行时

- Python
- OpenJDK
- Node.js

### 库

- glibc
- GLib
- OpenSSL
- OpenCV
- Mesa
- PowerVR

### Linux 内核

Linux 内核负责管理处理器和其他硬件资源，提供用户和应用程序与硬件之间的接口。主要功能包括：

- 中断和时钟管理
- 进程管理
- 内存管理
- 文件系统管理
- 设备驱动管理
- 网络协议栈

### 底层固件

底层固件包含 SPL、OpenSBI 和 UEFI：

- **SPL**：完成早期硬件初始化，并加载后续启动组件。
- **OpenSBI**：提供 RISC-V 监管二进制接口（SBI），并将启动控制权交给 UEFI。
- **UEFI**：从启动介质的 EFI 系统分区加载引导程序，再由引导程序启动 Linux 内核。

## 支持的设备

### K1

- MUSE Pi Pro

### K3

- Pico ITX
- COM260
