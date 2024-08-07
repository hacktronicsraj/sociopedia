FROM node:18-buster
WORKDIR /app
COPY /server/package.json ./
COPY /server/package-lock.json ./
RUN npm install
COPY . .
EXPOSE 5001
CMD ["npm", "run", "server"]