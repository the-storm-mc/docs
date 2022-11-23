VERSION 0.6

deps:
  FROM python:3.11
  RUN --secret=MKDOCS_GH_TOKEN=+secrets/sj/mkdocs_gh_token pip install git+https://${MKDOCS_GH_TOKEN}@github.com/squidfunk/mkdocs-material-insiders.git@8.5.10-insiders-4.26.3
  RUN pip install pillow cairosvg mkdocs-git-revision-date-localized-plugin mkdocs-git-authors-plugin mkdocs-glightbox

build:
  FROM +deps
  WORKDIR /workspace
  COPY . .
  RUN mkdocs build
  SAVE ARTIFACT site/* AS LOCAL out
