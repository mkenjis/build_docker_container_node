FROM mkenjis/mynode_img

RUN mkdir stuff
WORKDIR stuff

COPY helloworld.js .
COPY package.json .

RUN mkdir test
WORKDIR test
COPY helloworld_test.js .
RUN npm test