# 👋 你好，我是 Chen（晨）

> C++ / Linux / Backend / Storage / RPC  
> 关注存储引擎、高性能网络、RPC 框架与底层系统机制。

---

## 🧑‍💻 关于我

我是一名专注于 **C++ 后端与系统方向** 的在读研究生。  
相比只停留在业务开发，我更喜欢理解代码背后的运行机制：内存布局、线程调度、系统调用、缓存、网络 I/O、RPC 调用链路，以及数据库存储引擎的读写路径。

目前我正在深入学习和实践：

- **C++ 现代工程实践**：RAII、智能指针、移动语义、并发编程、性能分析
- **Linux 系统编程**：进程/线程、虚拟内存、IPC、网络编程、I/O 多路复用
- **存储与数据库内核**：LSM-Tree、WAL、MemTable、SSTable、Compaction、Block Cache
- **高性能后端基础设施**：RPC、事件驱动、异步 I/O、缓存策略、benchmark 与 profiling

---

## 🛠️ 技术栈

### Systems & Backend

![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-555555?style=for-the-badge&logo=c&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![RPC](https://img.shields.io/badge/RPC-1F2937?style=for-the-badge&logo=protocols.io&logoColor=white)

### Tools

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

---

## 🚀 正在构建的方向

### LevelDB-ScanAwareCache

基于 LevelDB 的读路径性能优化项目，关注范围扫描导致的 Block Cache 污染问题。

计划实现：

- LevelDB 读路径 metrics：SSTable 访问次数、Block Cache 命中率、Bloom Filter 过滤效果
- Scan-aware cache admission：降低范围扫描对热点缓存的污染
- YCSB-like benchmark：对比随机读、范围扫描、混合负载下的 P95/P99 延迟
- 技术报告：分析 LSM-Tree 中读放大、缓存污染与 Compaction 的关系

关键词：

```text
C++ / LevelDB / LSM-Tree / Block Cache / Bloom Filter / Compaction / Benchmark
```

### C++ RPC Framework

基于 C++ 的轻量级 RPC 框架项目，关注服务注册、网络通信、序列化、连接管理与高并发调用链路。

关注内容：

- Reactor 网络模型与事件循环
- TCP 连接管理、请求分发、超时控制
- RPC 服务注册、方法调用、序列化/反序列化
- 异步调用、线程池、负载均衡与压测分析

关键词：

```text
C++ / RPC / Reactor / TCP / Thread Pool / Serialization / Load Balance
```

---

## 📚 当前学习路线

```text
C++ 基础设施
├── Modern C++: RAII / move semantics / templates / concurrency
├── Linux: process / thread / mmap / epoll / IPC
├── Database: LevelDB / LSM-Tree / WAL / SSTable / Compaction
├── Network: TCP / Reactor / RPC / serialization / load balance
└── Performance: benchmark / perf / flamegraph / cache behavior
```

---

## 📊 GitHub 统计面板

> 外部统计图片有时会因为网络或第三方服务限制无法显示，所以这里使用稳定的文字版统计面板。后续项目成熟后，可以手动更新数据。

| 维度 | 当前重点 |
|---|---|
| 主语言 | C++ / C |
| 主攻方向 | 后端基础设施、存储引擎、RPC 框架 |
| 核心项目 | LevelDB-ScanAwareCache、C++ RPC Framework |
| 学习关键词 | Linux、LSM-Tree、Reactor、并发编程、性能优化 |
| 输出形式 | 源码实现、benchmark、技术报告、源码阅读笔记 |

```text
Current Focus
├── Storage Engine     ████████░░  LevelDB / LSM-Tree
├── RPC Framework      ███████░░░  Reactor / TCP / Thread Pool
├── Linux System       ██████░░░░  epoll / mmap / IPC
├── Modern C++         ███████░░░  RAII / concurrency / templates
└── Performance        ██████░░░░  benchmark / profiling / cache
```

---

## 🧭 我关注的问题

- 一个 key 在 LevelDB 中从 `Put` 到 `Get` 经历了什么？
- LSM-Tree 如何在读放大、写放大和空间放大之间做权衡？
- 一次 RPC 调用从 client stub 到 server method 经历了什么？
- Reactor、线程池和连接管理如何影响 RPC 框架的吞吐与延迟？
- C++ 如何写出既安全又高性能的系统级代码？
- 一个后端系统如何通过 benchmark 和 profiling 找到真正瓶颈？

---

## 📫 联系我

- GitHub: [coderchen02](https://github.com/coderchen02)
- 方向：C++ 后端开发 / Linux 系统编程 / 存储引擎 / RPC 框架

---

> 写代码时，我喜欢把问题拆到足够底层：数据在哪里，谁拥有它，什么时候释放，哪一步真正慢。
