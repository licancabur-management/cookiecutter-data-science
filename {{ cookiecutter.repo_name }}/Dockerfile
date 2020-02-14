FROM python:3.8.1-alpine
  RUN apk --no-cache add curl gcc musl-dev

  RUN mkdir -p /project

  WORKDIR /project

  RUN pip install --upgrade pip
  RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
  ENV PATH "$PATH:/root/.poetry/bin"
  RUN poetry config virtualenvs.path "/project_libs"

  COPY . .
