FROM python:3.6.4-slim

ENV PYTHONUNBUFFERED 1

RUN mkdir /code && apt-get update && apt-get install python-dev -y && apt-get install python3-dev -y && apt-get install gcc -y

WORKDIR /code

COPY . .

RUN pip install -r requirements.txt
