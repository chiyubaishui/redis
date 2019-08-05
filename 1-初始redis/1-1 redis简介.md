Redis是一种基于键值对（key-value）的NoSQL数据库。
Redis中的值可以是由string（字符串）、hash（哈希）、list（列表）、set（集合）、zset（有序集合）、Bitmaps（位图）、HyperLogLog、GEO（地理信息定位）等多种数据结构和算法组成。
Redis会将所有数据都存放在内存中，所以它的读写性能非常惊人。可以将内存的数据利用快照和日志的形式保存到硬盘上。
Redis还提供了键过期、发布订阅、事务、流水线、Lua脚本等附加功能。
