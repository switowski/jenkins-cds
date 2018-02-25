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
    # Pillow
    jpeg-dev \
    zlib-dev \
    libffi-dev \
    freetype-dev \
    libmspack-dev\
    libxml2-dev \
    libxslt-dev \
    libressl-dev \
    postgresql-dev \
    # Imagemagic 7 has a bug
    imagemagick6 \
    && pip install virtualenv \
    && rm -rf /var/cache/apk/*

USER jenkins
