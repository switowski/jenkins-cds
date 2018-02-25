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
    openssl-dev \
    && pip install virtualenv \
    && rm -rf /var/cache/apk/*

# Fix permissions
RUN npm config set user 0 \
    npm config set unsafe-perm true

USER jenkins
