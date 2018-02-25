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
    && curl -sL https://deb.nodesource.com/setup_9.x | bash - \
    && apk install -y nodejs \
    && pip install virtualenv \
    && rm -rf /var/cache/apk/*

USER jenkins
