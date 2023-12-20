FROM ghcr.io/eslih/python:3.12.0-alpine

WORKDIR /app

COPY ./requirements.txt ./

RUN apk add --no-cache libc6-compat

RUN pip install -r requirements.txt

COPY ./ ./

CMD ["python3", "app.py"]