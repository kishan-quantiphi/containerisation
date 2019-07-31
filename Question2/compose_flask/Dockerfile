FROM ubuntu:16.04
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
ADD . /code
WORKDIR /code
RUN pip install -r requirements.txt
CMD python app.py
