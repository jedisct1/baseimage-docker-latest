FROM ubuntu:15.04

ADD . /bd_build

RUN /bd_build/prepare.sh && \
	/bd_build/system_services.sh && \
	/bd_build/utilities.sh && \
	/bd_build/cleanup.sh

ENV TERM xterm

CMD ["/sbin/my_init"]
