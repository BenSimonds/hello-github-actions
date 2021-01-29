FROM python:3.8

COPY ./entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

WORKDIR /test

COPY ./requirements.txt /test/requirements.txt
COPY ./features /test/features

RUN pip install -r requirements.txt

ENTRYPOINT /entrypoint.sh
