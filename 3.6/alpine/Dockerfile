FROM python:3.6-alpine

LABEL maintainer "Mathieu Lemay <acidrain1@gmail.com>"

RUN apk add --no-cache --virtual .deps curl && \
    curl -sSL https://raw.githubusercontent.com/sdispater/poetry/master/get-poetry.py | python && \
    apk del --no-cache .deps

ENV PATH="/root/.poetry/bin:$PATH"
