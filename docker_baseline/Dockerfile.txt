FROM ubuntu
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update \
 && apt-get install -y tzdata \
 && apt-get install -y npm \
 && apt-get install -y nodejs

RUN npm init --yes
RUN npm install mocha@2.5.3 --save-dev
RUN npm install zombie --save-dev