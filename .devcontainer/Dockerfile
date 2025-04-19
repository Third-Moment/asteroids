FROM mcr.microsoft.com/devcontainers/python:1-3.12-bullseye

RUN apt-get update && apt-get install -y --no-install-recommends \
    libx11-dev \
    libxext-dev \
    libxrender-dev \
    libxtst-dev \
    x11-apps \
    && rm -rf /var/lib/apt/lists/*

COPY requirements.txt /tmp/

RUN pip install --no-cache-dir -r /tmp/requirements.txt