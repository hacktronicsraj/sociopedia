FROM 22-alpine3.19
WORKDIR /app
COPY /server/package.json ./
COPY /server/package-lock.json ./
RUN npm install
COPY ./server .
EXPOSE 5001
CMD ["npm", "run", "server"]