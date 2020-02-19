FROM amazonlinux:2

RUN yum -y update

RUN yum -y install \
    groff          \
    less           \
    mailcap        \
    unzip

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "aws-cli-v2.zip"
RUN unzip "aws-cli-v2.zip"
RUN rm "aws-cli-v2.zip"
RUN ./aws/install

CMD ["/bin/sh"]
