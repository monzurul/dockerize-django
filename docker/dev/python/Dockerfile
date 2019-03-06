FROM python:3.5
MAINTAINER oametrix@localhost

COPY ./oametrix2019/openaccess /app

WORKDIR /app

RUN pip install -r requirements.txt
#RUN python manage.py migrate
#RUN python manage.py openaccess_init_data
#RUN python manage.py openaccess_init_data2

COPY ./docker/dev/python/entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
