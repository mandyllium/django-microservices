FROM python:3.6.4-slim

ENV PYTHONUNBUFFERED 1

RUN mkdir /code && apt-get update && apt-get install python-dev -y && apt-get install python3-dev -y && apt-get install libpq-dev -y && apt-get install gcc -y && unlink /usr/local/bin/python3 && ln -s /usr/local/bin/python3.6 /usr/local/bin/python3

WORKDIR /code

COPY . .

RUN pip install -r requirements.txt
