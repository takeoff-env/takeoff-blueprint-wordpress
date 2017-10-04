FROM nginx:1.10-alpine

RUN mkdir -p /home/wordpress/wordpress
WORKDIR /home/wordpress/wordpress

COPY /env/nginx/conf/nginx.conf /etc/nginx/conf.d/default.conf

COPY . ./
