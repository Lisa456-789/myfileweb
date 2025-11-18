---
title: 数据结构
---

# 数据结构

# 复杂度

- 时间：O(1)、O(log n)、O(n)、O(n log n)、O(n²)
- 空间：递归、缓存与持久化结构

# 线性结构

- 数组与链表
- 栈与队列、双端队列

# 树与图

- 二叉搜索树、AVL、红黑树
- 图的表示：邻接表、邻接矩阵
- 遍历：BFS、DFS

# 堆与优先队列

- 二叉堆、斐波那契堆
- Top-K 与调度

# 哈希结构

- 开放寻址与链式地址
- 一致性哈希与分片

# 示例：二分查找

```js
function bs(a, t) {
  let l = 0, r = a.length - 1
  while (l <= r) {
    const m = (l + r) >> 1
    if (a[m] === t) return m
    if (a[m] < t) l = m + 1
    else r = m - 1
  }
  return -1
}
```