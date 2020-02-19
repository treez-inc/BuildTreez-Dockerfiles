FROM ubuntu:18.04

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y \
    curl  \
    groff \
    less  \
    unzip

WORKDIR /root

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN ./aws/install

CMD ["/bin/sh"]
