FROM balenalib/raspberrypi4-64-alpine-node

WORKDIR /usr/src/app
COPY package.json package-lock.json ./
COPY ./lib ./lib
RUN npm i
RUN pwd && ls -al && ls -al lib

CMD ["node", "lib/index.js"]
