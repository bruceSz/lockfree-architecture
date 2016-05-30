可扩展性系统

1 可扩展系统分为三层： 高层架构，中层设计，底层实现
2 设计房屋和程序设计一样；多核cpu和一个集群一样
3 解决扩展问题的两个方法： 去中心化；独立（去依赖）。
4 中心化意味着最优决策，在分布式系统中则意味着更多的communication（同步），互斥。。
5 去中心化意味着局部最优决策，因为没有全局信息，全局最优不能达到。并且复杂性上升。
6 依赖意味着减少并发。
7 去依赖基本方法： mvcc，参考实现：http://www.1024cores.net/home/lock-free-algorithms/object-life-time-management/differential-reference-counting
8 basically thread-safe: 并发读，互斥写；strong thread-safe: 并发读写
9 