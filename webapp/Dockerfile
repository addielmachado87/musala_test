FROM node:alpine


COPY . /srv/

WORKDIR /srv

RUN npm install -g @angular/cli

RUN npm i

RUN ng build

EXPOSE 4200

CMD ["npm", "run", "start" ]



# to production
#FROM nginx:1.13.12-alpine as production-stage
#COPY --from=build-stage /app/dist /usr/share/nginx/html
#COPY deploy/nginx/default.conf /etc/nginx/conf.d/default.conf
#EXPOSE 80
#CMD ["nginx", "-g", "daemon off;"]
