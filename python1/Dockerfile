FROM python:3.11 as builder
RUN mkdir /usr/src/app
COPY ./my-app /usr/src/app
COPY ./requirements.txt /usr/src/app

WORKDIR /usr/src/app

RUN pip install --no-cache-dir -r requirements.txt
EXPOSE 5000
CMD [ "python", "app.py" ]