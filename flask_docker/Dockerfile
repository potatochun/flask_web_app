FROM tiangolo/uwsgi-nginx-flask:python3.6

COPY ./app /app

COPY ./Pip* /app/

RUN pip install --upgrade pip && pip install pipenv && pipenv install --dev --system --ignore-pipfile --deploy

