# We are using alpine
FROM python:alpine AS base

COPY ./pet-board /service
WORKDIR /service

RUN pip3 install -r requirements.txt

EXPOSE 5000

WORKDIR /service/demo-ui
ENTRYPOINT ["python3"]
CMD ["__init__.py"]