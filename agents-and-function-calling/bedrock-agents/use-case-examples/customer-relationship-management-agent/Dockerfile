FROM public.ecr.aws/docker/library/python:3.9-slim

WORKDIR /frontend

RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    software-properties-common \
    xclip \
    xselect \
    git \
    && rm -rf /var/lib/apt/lists/*

sudo apt-get install 
COPY . .

RUN pip3 install -r requirements.txt

EXPOSE 80
