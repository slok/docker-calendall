FROM python:3.4.2
MAINTAINER Xabier Larrakoetxea <slok69@gmail.com>


RUN apt-get update && \
    apt-get -y -q install git\
                  libpq5\
                  libpq-dev

RUN git clone https://github.com/calendall/calendall.git /tmp/calendall
RUN pip install -r /tmp/calendall/requirements/dev.txt
RUN rm -rf /tmp/calendall

RUN mkdir /code
WORKDIR /code

EXPOSE 8000
VOLUME /data
