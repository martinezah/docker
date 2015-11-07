FROM martinezah/supervisor
MAINTAINER "Marti Martinez" <martinezah@gmail.com>

RUN apt-get install -y redis-server
ADD supervisor/redis.conf /etc/supervisord.d
ADD redis.conf /etc
RUN mkdir /data 
RUN chown redis:redis /data
VOLUME /data

EXPOSE 6379
