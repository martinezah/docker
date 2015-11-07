FROM martinezah/ubuntu-python
MAINTAINER "Marti Martinez" <martinezah@gmail.com>

RUN pip install supervisor
ADD supervisord.conf /etc/
RUN mkdir /etc/supervisord.d

EXPOSE 9001
ENTRYPOINT ["/usr/local/bin/supervisord"] 
CMD ["-c", "/etc/supervisord.conf"]
