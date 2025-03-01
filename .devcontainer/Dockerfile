FROM mcr.microsoft.com/devcontainers/python:1-3.12-bullseye

RUN python3 -m venv /opt/pipx-venv && \
    /opt/pipx-venv/bin/pip install pipx && \
    /opt/pipx-venv/bin/pipx ensurepath

RUN pipx install poetry

RUN usermod -aG root vscode

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends docker.io