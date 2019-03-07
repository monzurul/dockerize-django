FROM nginx:latest

RUN rm /etc/nginx/conf.d/default.conf

COPY ./react_oametrix/build /app

WORKDIR /app

COPY ./docker/dev/frontend/site.conf /etc/nginx/conf.d/




