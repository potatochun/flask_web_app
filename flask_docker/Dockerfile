FROM tiangolo/uwsgi-nginx-flask:python2.7

COPY ./app /app
COPY ./requirements.txt /app

RUN pip install -r /app/requirements.txt
