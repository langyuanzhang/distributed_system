### 分布式系统概念

> 旨在支持应用程序和服务的开发，可以利用物理架构有*多个自治的处理元素*，*不共享主内存*，但通过*网络发送消息*合作。 ——*Leslie Lamport*

#### 三个特点和三个概念

* ###### 三个特点
1. 多节点
2. 消息通信
3. 不共享内存

* ###### 三个概念
1. 分布式系统
_分布式系统是每个节点中有不同的功能模块，所有节点组合构成一个程序。 分布式系统各个节点是通过发送消息来通信的，比如 http、RESTful接口、RPC。_

2. 集群
_集群是多个节点中有相同的程序_

3. 分布式计算
_分布式计算有些地方叫并行计算，如hadoop中的hadoop mapreduce。分布式计算是该功能有多个执行，整合得出一个结果_

#### 联系
分布式系统是多节点的，集群也是多节点的

#### 区别
分布式强调的是不同功能模块的节点，而集群指的是相同业务功能的节点。
分布式中的每个节点都可以做集群，群集的规模由这个业务的规模所决定。
集群并不一定是分布式的，比如前后端未分离的系统，所有的业务模块都在一起，就算它有所有机器做了集群，但是这些节点并不需要进行消息通信，所以它并不是分布式的。

