FROM amazonlinux:latest

RUN yum -y install  python3 \
    python3-pip \
    zip \
    && yum clean all

RUN python3 -m pip install --upgrade pip \
   && python3 -m pip install boto3