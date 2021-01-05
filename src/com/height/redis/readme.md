## Redis分布式锁解读

### 1.分布式锁需求说明
  - 独占性：一个时间只能最多有一个线程能获取到锁。
  - 解锁控制：当持有锁的线程正常执行时，只有当前持有锁的线程才能解锁，不能被其他线程解锁或者自动失效。
  - 解锁容错：当尺有所的线程崩溃或异常中断时，有机制能释放锁。
  - 集群容错：当Redis主节点获取到锁信息时，可能未完成锁信息的从节点同步就崩溃了，可能会导致锁信息丢失。

### 2.常见分布式锁的问题
    
### 3.Redisson实现

### 4.Redisson源码解读