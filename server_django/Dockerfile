FROM python:3.12.2-slim-bullseye

ENV PYTHONUNBUFFERED=1

WORKDIR /app

COPY . /app/

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

CMD gunicorn core.wsgi:application --bind 0.0.0.0:8000