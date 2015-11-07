FROM martinezah/ubuntu-python

MAINTAINER "Marti Martinez" <martinezah@gmail.com>

RUN pip install supervisor
ADD supervisord.conf /etc/

ENTRYPOINT ["/usr/local/bin/supervisord"] 

CMD ["-c", "/etc/supervisord.conf"]
