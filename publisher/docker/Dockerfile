FROM python:3.6

ENV PYTHONUNBUFFERED 1

ARG debug
ENV DEBUG=$debug

RUN mkdir -p /config
ADD requirements.txt /config/

RUN pip install -r /config/requirements.txt

RUN mkdir -p /src
COPY . /src
WORKDIR /src
