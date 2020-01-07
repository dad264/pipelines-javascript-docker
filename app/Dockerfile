FROM node:8

RUN cd /tmp && echo "hello!"

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm ci --only=production

COPY . .

EXPOSE 8080
CMD [ "npm", "start" ]