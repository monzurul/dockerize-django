FROM python:3.5
MAINTAINER oametrix@localhost

COPY ./oametrix2019/openaccess /app

WORKDIR /app

RUN pip install -r requirements.txt


COPY ./docker/dev/backend/entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
