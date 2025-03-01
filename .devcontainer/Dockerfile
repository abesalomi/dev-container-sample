FROM mcr.microsoft.com/devcontainers/python:1-3.12-bullseye

RUN python3 -m venv /opt/pipx-venv && \
    /opt/pipx-venv/bin/pip install pipx && \
    /opt/pipx-venv/bin/pipx ensurepath

RUN pipx install poetry