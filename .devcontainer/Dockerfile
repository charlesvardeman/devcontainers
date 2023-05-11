FROM mcr.microsoft.com/devcontainers/python:3

RUN python -m pip install --upgrade pip \
    && python -m pip install 'pdm' \ 
    && python -m pip install 'dvc>=2.56.0' \
    && python -m pip install 'dvclive>=2.5.1' \
    && python -m pip install 'nbdev>=1.1.5'

ENV FLIT_ROOT_INSTALL=1

COPY pyproject.toml .
RUN python -m pdm install
