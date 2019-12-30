FROM python:3.7-alpine
MAINTAINER StyleZ

ENV PYTHONUNBUFFERED 1

RUN mkdir /app
WORKDIR /app
COPY ./app /app
RUN pip install -r ./requirements.txt

RUN adduser -D user
USER user
EXPOSE 8080/tcp
