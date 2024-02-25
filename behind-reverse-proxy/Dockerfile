FROM nginx:1.24.0-alpine

RUN apk update \
    && apk add dcron \
    && apk add bash

COPY 81.nginx /etc/nginx/nginx.conf
COPY index.html /usr/share/nginx/html
EXPOSE 81
CMD ["nginx", "-g", "daemon off;"]


