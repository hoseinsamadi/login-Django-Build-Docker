FROM python:3.11.4-alpine

WORKDIR /app

RUN pip install --upgrade pip
COPY ./requirements.txt app/requirements.txt
RUN pip install -r requirements.txt
COPY ./enterypoint.sh /app/enterypoint.sh

COPY . app/

ENTRYPOINT [ "/app/enterypoint.sh" ]