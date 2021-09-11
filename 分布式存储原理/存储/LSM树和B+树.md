### LSM树

LSM树，全称是The Log-Structured Merge-Tree (LSM-Tree)

这里面有两个重点 Log-Structured 和 Merge-Tree， Merge-Tree说明了它不是一个简单的树

LSM-tree 是专门为 key-value 存储系统设计的，LSM-tree 最大的特点就是写入速度快，主要利用了
磁盘的顺序写，pk掉了需要随机写入的 B-tree

LSM-tree 被用在各种键值数据库中，如 LevelDB，RocksDB，还有分布式行式存储数据库 Cassandra
也用了 LSM-tree 的存储架构
