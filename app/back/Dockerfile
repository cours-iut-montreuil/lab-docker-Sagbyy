FROM python:latest

WORKDIR /app

COPY  . /app

RUN mkdir logs

RUN pip install -r requirements.txt

CMD [ "uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8080"]