# Select a base image
FROM  node:latest

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 5555

CMD ["npm", "start","--","--host","0.0.0.0"]