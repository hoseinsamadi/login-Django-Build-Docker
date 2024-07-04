FROM python:3.9.19-alpine3.20

WORKDIR /app

RUN pip install --upgrade pip
COPY ../Django-Login/requirements.txt app/requirements.txt
RUN pip install -r requirements.txt
COPY ./entrypoint.sh /app/entrypoint.sh

COPY . app/

ENTRYPOINT [ "/app/entrypoint.sh" ]