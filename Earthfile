VERSION 0.6

deps:
  FROM python:3.11
  RUN pip install pipenv
  COPY Pipfile* .
  RUN --secret=MKDOCS_GH_TOKEN=+secrets/sj/mkdocs_gh_token pipenv install

build:
  FROM +deps
  WORKDIR /workspace
  COPY docs docs
  COPY mkdocs.yml .
  # Required for committer information
  COPY .git .git
  RUN pipenv run mkdocs build
  SAVE ARTIFACT site/*

dev:
  LOCALLY
  RUN pipenv run mkdocs serve
