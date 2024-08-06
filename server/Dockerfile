From node:16-buster

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY package*.json /usr/src/app/

RUN npm NODE_ENV=development ci

COPY . /usr/src/app

EXPOSE 5001

CMD ["npm", "run", "server"]