FROM node:16
WORKDIR /app
COPY /server/package.json ./
COPY /server/package-lock.json ./
RUN npm install
COPY ./server .
EXPOSE 5001
CMD ["npm", "run", "server"]