FROM python:3.8.0
FROM ubuntu:latest

ENV LANG=C.UTF-8
ENV DEBIAN_FRONTEND=noninteractive

WORKDIR /usr/src/flask_app
COPY requirements.txt .
RUN apt-get update
RUN apt-get install -y python3-pip

COPY . .

RUN echo server will be running on 5000

RUN pip install --no-cache-dir -r requirements.txt

CMD ["python3", "app.py"]                    
