# 👋 你好，我是 Chen（晨）

> C++ 后端开发 · Linux 系统编程 · 计算机网络

我是一名在读研究生，主要学习和实践 **C++ 后端与系统编程**。目前围绕 **多 Reactor 服务器** 和 **RPC 框架** 开展项目，通过代码理解网络通信、线程协作与资源管理。

## 🛠️ 技术栈与学习方向

![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

- **C++**：面向对象、STL、RAII、智能指针、移动语义与并发编程。
- **操作系统与 Linux**：进程与线程、虚拟内存、线程同步、进程间通信和系统调用。
- **计算机网络**：TCP/IP、HTTP/HTTPS、Socket 编程、I/O 多路复用与 Reactor 模型。

## 🚀 项目实践

### [多 Reactor 网络服务器](https://github.com/coderchen02/multi-reactor-server)

基于 C++ 的多 Reactor HTTP 服务器项目，围绕连接建立、事件分发、网络读写和 HTTP 请求处理组织代码。

- **主从 Reactor**：主 Reactor 接收新连接，将连接分配给工作线程中的子 Reactor。
- **事件驱动设计**：通过 `EventLoop`、`Channel` 和 `Dispatcher` 组织事件循环与 I/O 多路复用。
- **连接与协议处理**：封装 TCP 连接、读写缓冲区、HTTP 请求解析和响应生成。

`C++` · `Linux` · `TCP` · `Reactor` · `epoll` · `多线程` · `HTTP`

### [C++ RPC 框架](https://github.com/coderchen02/rpc)

基于 C++ 的 RPC 框架项目，打通服务发现、节点选择、请求序列化、网络传输和远程方法调用的链路。

- **通信与序列化**：使用 TCP 传输请求和响应，通过 Protobuf 编码调用信息及参数。
- **服务注册与发现**：通过 ZooKeeper 管理服务实例，结合客户端本地缓存获取可用节点。
- **客户端负载均衡**：从可用实例中选择目标节点，分发远程调用请求。
- **调用可靠性**：围绕响应超时、故障节点隔离和幂等方法重试处理调用失败。

`C++` · `RPC` · `TCP` · `Protobuf` · `ZooKeeper` · `服务发现` · `负载均衡`

## 📚 学习记录

- [C++ 基础与代码练习](https://github.com/coderchen02/Cplusplus-basis-syntax)
- [计算机网络学习笔记](https://github.com/coderchen02/computer-network-learning)
- [算法练习](https://github.com/coderchen02/AcWingBasicAlgorithm)

## 📫 联系我

- Email：[hanchen200205@163.com](mailto:hanchen200205@163.com)
- 方向：C++ 后端开发 / Linux 系统编程 / 网络编程 / RPC 框架

---

> 我关心代码背后的机制：数据由谁管理，线程如何协作，请求如何完成一次往返。
