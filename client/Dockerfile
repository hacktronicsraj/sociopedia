FROM node:18-buster
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY /client/package.json /app/package.json
COPY /client/package-lock.json /app/package-lock.json
COPY /client/package*.json /usr/src/app/
RUN npm install
COPY ./client /usr/src/app/
EXPOSE 3000
CMD ["npm", "start"]