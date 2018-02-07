FROM node:alpine

RUN apk add --update git openssh
RUN git clone https://github.com/JulHorn/image_diff_server.git imageDiffServer
WORKDIR  /imageDiffServer
COPY default.json ./config
RUN npm install

CMD npm start