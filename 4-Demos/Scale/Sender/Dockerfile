FROM ubuntu:16.04
MAINTAINER Matheus Fidelis <msfidelis01@gmail.com>

RUN apt-get update && apt-get install python-pip -y
RUN pip install pika
RUN mkdir /app

COPY sender.py /app/sender.py
WORKDIR /app

CMD ["python", "sender.py"]
