FROM python:3

MAINTAINER Alexandre Frydman "@@epitech.eu"

RUN apt-get update -y && \
    apt-get install -y python3-pip python3-dev

COPY requirements.txt /app/requirements.txt

WORKDIR /app

COPY . /app

RUN pip3 install -r requirements.txt

EXPOSE 80

ENTRYPOINT [ "python3" ]

CMD [ "app.py" ]