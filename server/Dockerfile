FROM node:16-buster
WORKDIR /app
COPY package.json ./
COPY package-lock.json ./
RUN npm install
COPY . .
EXPOSE 5001
CMD ["npm", "run", "server"]