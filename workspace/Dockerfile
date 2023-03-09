# Dockerfile
FROM python:3.9
LABEL version, description
WORKDIR /data/app
COPY . /data/app
RUN python -m pip install --upgrade pip
RUN pip install -r requirements.txt
