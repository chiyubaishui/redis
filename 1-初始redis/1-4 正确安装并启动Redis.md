1����װ��
$ wget http://download.redis.io/releases/redis-3.0.7.tar.gz
$ tar xzf redis-3.0.7.tar.gz
$ ln -s redis-3.0.7 redis
$ cd redis
$ make
$ make install
2������Redis�������ļ�����
# redis-server /opt/redis/redis.conf
3��Redis�����пͻ��ˣ�����ʽ��ʽ��ͨ��redis-cli-h{host}-p{port}�ķ�ʽ���ӵ�Redis
����
redis-cli -h 127.0.0.1 -p 6379
4��ֹͣRedis����
$ redis-cli shutdown
���Կ���Redis����־������£�
# User requested shutdown... #�ͻ��˷�����shutdown����
* Saving the final RDB snapshot before exiting.
#����RDB�־û��ļ�(�й�Redis�־û���������1.2���Ѿ������˼򵥵Ľ��ܣ�RDB��Redis��һ��
�־û���ʽ)
* DB saved on disk #��RDB�ļ������ڴ�����
# Redis is now ready to exit, bye bye... #�ر�