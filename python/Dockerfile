# https://hub.docker.com/_/python
FROM python:3.10-slim

WORKDIR /app
COPY . ./

# Installing the dependencies for the python code.
RUN pip install -r requirements.txt

CMD uvicorn main:app --port $PORT --workers 1 --host 0.0.0.0
