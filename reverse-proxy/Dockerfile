FROM nginx:1.24.0-alpine

RUN apk update \
    && apk add dcron 

COPY 80.nginx /etc/nginx/nginx.conf
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]


