FROM python:3.9-slim

WORKDIR /app

COPY . .

RUN pip install Flask
RUN pip install gunicorn

CMD gunicorn --bind 0.0.0.0:5000 wsgi:app
