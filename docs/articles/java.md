---
title: Java
---

# Java

# 概述

Java 生态成熟，跨平台、稳定，适合后端服务与大型系统。本文整理语言基础、并发、JVM 调优与常用库。

# 开发环境

- JDK 17
- 构建工具：Maven 或 Gradle
- IDE：IntelliJ IDEA

# 基础语法速览

```java
public class Hello {
  public static void main(String[] args) {
    System.out.println("Hello");
  }
}
```

# 面向对象与集合

- 接口与抽象类
- 集合：List、Set、Map
- Stream 与 Optional

# 并发与线程安全

- Executors 与线程池
- 原子类与锁
- 并发集合

# JVM 与性能

- 内存结构：堆、栈、方法区
- 垃圾回收：G1、ZGC
- 工具：jps、jstack、jmap、jstat

# 示例：并发计数

```java
import java.util.concurrent.*;

class Counter {
  private final ExecutorService pool = Executors.newFixedThreadPool(4);
  public Future<Integer> calc(int n) {
    return pool.submit(() -> {
      int s = 0;
      for (int i = 0; i < n; i++) s += i;
      return s;
    });
  }
}
```

# 推荐库

- Spring Boot、Spring Cloud
- Lombok、Guava
- Jackson、MapStruct