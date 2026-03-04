FROM nginx:alpine

# Patch ALL known vulnerabilities at build time
RUN apk update && apk upgrade --no-cache

# Remove default Nginx page and copy our app
RUN rm -rf /usr/share/nginx/html/*
COPY . /usr/share/nginx/html/

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

