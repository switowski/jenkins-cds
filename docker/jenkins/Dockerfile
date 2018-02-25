FROM jenkinsci/blueocean:latest

USER root

RUN apk add --no-cache --update \
    python \
    python-dev \
    py-pip \
    build-base \
    curl \
    git \
    gcc \
    nodejs \
    nodejs-npm \
    libffi-dev \
    libxml2-dev \
    libxslt-dev \
    libressl-dev \
    postgresql-dev \
    imagemagick \
    && pip install virtualenv \
    && rm -rf /var/cache/apk/*

USER jenkins
