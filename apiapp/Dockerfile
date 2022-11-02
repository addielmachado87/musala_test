FROM node:alpine

COPY . /srv/

WORKDIR /srv

RUN npm install

EXPOSE 80

CMD [ "npm", "run","dev" ]
