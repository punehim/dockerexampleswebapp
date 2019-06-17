FROM ubuntu

RUN apt-get update
RUN apt-get install -y python python-pip
RUN pip install flask

COPY webapp.py /opt/webapp.py

ENTRYPOINT FLASK_APP=/opt/webapp.py flask run --host=0.0.0.0
