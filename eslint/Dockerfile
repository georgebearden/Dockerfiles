FROM amazonlinux:latest

ADD . .

RUN curl -sL https://rpm.nodesource.com/setup_8.x | bash -
RUN yum -y install nodejs

RUN npm install -g eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react