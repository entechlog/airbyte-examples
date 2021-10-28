# Dockerfile
FROM python:3.9-slim-buster

WORKDIR /usr/app

COPY requirements.txt ./

# Install Python Requirements
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y --no-install-recommends git curl && \
    apt-get purge -y --auto-remove

# Install Docker
RUN apt-get update && \
    apt-get -qy full-upgrade && \
    apt-get install -qy curl && \
    apt-get install -qy curl && \
    curl -sSL https://get.docker.com/ | sh

RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

CMD ["docker", "--version"]