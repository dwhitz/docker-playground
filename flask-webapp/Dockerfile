FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y python 
RUN apt-get install -y python-pip
RUN pip install flask

COPY app/ /opt/app

ENTRYPOINT FLASK_APP=/opt/app/app.py flask run --host=0.0.0.0 --port=8080

