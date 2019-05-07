FROM amazonlinux:latest

RUN yum -y install tar \
    gzip \
    && yum clean all

RUN touch ~/.bashrc
RUN curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.32.0/install.sh | bash
RUN /bin/bash -c ". ~/.nvm/nvm.sh && nvm install 8.10"