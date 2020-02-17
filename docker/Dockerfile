FROM nginx:latest

RUN apt-get update && \
    apt-get -y upgrade

COPY ./build /var/www
COPY nginx.conf /etc/nginx/nginx.conf

RUN rm -rf /var/lib/apt/lists/*

EXPOSE 80

WORKDIR /var/www
