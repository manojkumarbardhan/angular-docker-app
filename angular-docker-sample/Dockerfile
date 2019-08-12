#Base Image
FROM nginx:1.17.2-alpine

## Copy our default nginx config
COPY nginx.conf /etc/nginx/conf.d/

RUN rm -rf /usr/share/nginx/html/*
COPY /dist/angular-docker-sample /usr/share/nginx/html/

CMD ["nginx", "-g", "daemon off;"]