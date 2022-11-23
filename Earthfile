VERSION 0.6

deps:
  FROM python:3.11
  RUN --secret=MKDOCS_GH_TOKEN=+secrets/sj/mkdocs_gh_token pip install git+https://${MKDOCS_GH_TOKEN}@github.com/squidfunk/mkdocs-material-insiders.git@8.5.10-insiders-4.26.3

build:
  FROM +deps
  WORKDIR /workspace
  COPY . .
  RUN mkdocs build
  SAVE ARTIFACT site/* AS LOCAL out
