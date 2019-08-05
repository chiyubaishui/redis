1、安装：
$ wget http://download.redis.io/releases/redis-3.0.7.tar.gz
$ tar xzf redis-3.0.7.tar.gz
$ ln -s redis-3.0.7 redis
$ cd redis
$ make
$ make install
2、启动Redis：配置文件启动
# redis-server /opt/redis/redis.conf
3、Redis命令行客户端：交互式方式：通过redis-cli-h{host}-p{port}的方式连接到Redis
服务
redis-cli -h 127.0.0.1 -p 6379
4、停止Redis服务：
$ redis-cli shutdown
可以看到Redis的日志输出如下：
# User requested shutdown... #客户端发出的shutdown命令
* Saving the final RDB snapshot before exiting.
#保存RDB持久化文件(有关Redis持久化的特性在1.2节已经进行了简单的介绍，RDB是Redis的一种
持久化方式)
* DB saved on disk #将RDB文件保存在磁盘上
# Redis is now ready to exit, bye bye... #关闭