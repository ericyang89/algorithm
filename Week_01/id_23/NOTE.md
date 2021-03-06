# 算法训练营总结

## 算法之外

1. 学习是反人性的，可以通过刻意练习来解决难的知识点。
2. 数据结构中数组 不等于 编程语言中的数组。一些其他的结构，在不通的语言中也不完全一样；但一般具有一定的相似性。
3. 尾递归优化不是解决 递归异常（stackoverflow）的万金油。原因一：需要语言支持；原因二：不是所有递归都能专成尾递归。
4. 数学主要学的是方法，结果无法穷举，唯有掌握方法。掌握方法可以通过反复的训练来解决。（所以需要做大量的数学题）。
5. 解决问题的思路：

  + 需求分享（读题）
  + 找解决思路（确定相应的数据结构和算法，先找对数据结构）
  + 如果思路不明确，可以求助。求助的时候需要说出自己的思路和做过哪些努力。
  + 写代码。（写代码前可以将思路转成图）

## 经典问题的套路

1. 大量数据（无法完全加载到 内存），可以分治，类似map reduce。
2. 链表问题一般思路比较简单，主要很多边界问题。需要通过多编码解决。
3. 数组相关问题，一般解决性能优化。O(n^2)-->O(n*logn)，第一层遍历无法避免，第二层是否可优化成 logn;有序数组查找一般采用二分法。
4. 字符串处理，一般都需要遍历，有限的字符集查询，使用hash；公共前缀的用 trie 树。
5. 二叉树一般用递归实现。
6. 部分问题，需要使用多种数据结构或算法。LRU cache，hash table+ 链表。

## 相关知识点

1. 排序的稳定性：相同的数据，在排序前后，前后顺序不变。
2. 排序的愿地性：假设 n 个数排序，不另外需要一个n 相关的存储空间。
3. 常规图可以矩阵存储；在内存中，稀疏图可用邻接表或逆邻接表存储（比喻 好友关系）。持久化数据，可用图数据库或者常规关系数据库。
4. 动态规划的解法核心：找到最优字结构，推导出状态转移方程。
5. 动态规划优势，减少重复字问题的重复计算。
6. 数据库索引 B+ tree；
7. redis set 实现 使用跳表。链表建多级索引。空间复杂度索引翻倍；时间复杂度，logn。
8. 映射陷阱，易忽略双向映射。
9. 递归=递推公式+退出条件。