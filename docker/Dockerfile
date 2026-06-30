FROM python:3.13-slim

RUN apt-get update && apt-get install git -y && rm -rf /var/lib/apt/lists/*
COPY requirements.txt /dependencies/requirements.txt
RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r /dependencies/requirements.txt
WORKDIR /home/app
