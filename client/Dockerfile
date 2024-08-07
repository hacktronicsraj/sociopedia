FROM node:16-buster
WORKDIR /app
COPY /client/package.json ./
COPY /client/package-lock.json ./
RUN npm install
RUN npm ci --only=production
COPY ./client .
EXPOSE 3000
CMD ["npm", "start"]