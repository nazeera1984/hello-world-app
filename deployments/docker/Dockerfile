## base image should be python:3
FROM python:3

## we should copy all files to the image
COPY  . /app

## Default folder for the image /app
WORKDIR /app

## Expose 5000 port for the app
EXPOSE 5000

## Install all libraries
RUN pip install -r requirements.txt

## Make sure when containers started and application will be started as well
CMD [ "/bin/sh", "-c", "python /app/app.py" ]
