{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

- Intalling packages: docker-compose run app poetry install
- Running the formatter: docker-compose run app poetry run black src/
- Running the linter: docker-compose run app poetry run flake8 src/
