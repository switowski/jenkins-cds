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
    libjpeg-dev \
    libffi-dev \
    libfreetype6-dev \
    libmsgpack-dev \
    # CairoSVG
    libcairo2-dev \
    libssl-dev \
    libxml2-dev \
    libxslt-dev \
    imagemagick \
    && pip install virtualenv \
    && rm -rf /var/cache/apk/*

USER jenkins
