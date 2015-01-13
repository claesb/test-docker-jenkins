FROM schibstedpayment/oracle-java-8

MAINTAINER Claes Bergsten <claes@spid.no>

ENV WORKDIR /srv/test

RUN mkdir -p $WORKDIR

EXPOSE 8080

ADD target/* $WORKDIR/
ADD start.sh $$WORKDIR/
RUN chmod +x $$WORKDIR/start.sh

CMD $PMAHOME/start.sh