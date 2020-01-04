FROM python:3.8.1-alpine
  RUN apk --no-cache add curl

  RUN mkdir -p /project

  WORKDIR /project

  RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
  ENV PATH "$PATH:/root/.poetry/bin"
