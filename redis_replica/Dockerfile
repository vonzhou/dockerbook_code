FROM vonzhou/redis

ENTRYPOINT [ "redis-server", "--protected-mode no", "--logfile /var/log/redis/redis-replica.log", "--slaveof redis_primary 6379" ]

