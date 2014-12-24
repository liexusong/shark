1. shark简介
  shark是一个高性能的协程网络组建, 可以使用同步的方式编写高性能异步的网络程序. 
  shark适合需要使用epoll处理大量并发tcp连接的场景，性能与裸用epoll相当.
  shark在不降低性能的基础上，大大降低使用C++编写高性能网络程序的难度，使用简单的几个接口就可以构建高性能的网络程序.

2. shark特性
1)	同步无锁方式编写高性能异步代码
2)	支持多核, 支持核心绑定
3)	支持多进程并行计算, 支持进程间负载均衡
4)	Hook并优化阻塞的网络系统调用, 让第三方组件同步变异步
5)	支持动态协程池, 汇编实现的高性能协程上下文切换, 每秒达1.7亿次
6)	高效的超时机制, 支持千万级timer
7)	高性能的缓存机制
8)	支持连接池, mysql