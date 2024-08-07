FROM node:18-buster
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY /server/package.json /app/package.json
COPY /server/package-lock.json /app/package-lock.json
COPY /server/package*.json /usr/src/app/
RUN npm install
COPY ./server /usr/src/app/
EXPOSE 5001
CMD ["npm", "run", "server"]