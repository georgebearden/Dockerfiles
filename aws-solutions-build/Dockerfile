FROM amazonlinux:latest

RUN yum -y install tar \
    zip \
    unzip \
    gzip \
    rsync \
    dos2unix \
    && yum clean all

RUN touch ~/.bashrc
RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.2/install.sh | bash
RUN /bin/bash -c ". ~/.nvm/nvm.sh && nvm install 12"