FROM nginx:1.27-alpine3.20

RUN apk update && apk upgrade --no-cache

RUN rm -rf /usr/share/nginx/html/*
COPY . /usr/share/nginx/html/

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

