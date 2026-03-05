FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN apt-get update && apt-get install -y \
    libgtk-3-0 \
    libnotify-dev \
    libnss3 \
    libxss1 \
    libasound2t64 \
    libxtst6 \
    libatspi2.0-0 \
    libdrm2 \
    libgbm1 \
    xvfb \
    && rm -rf /var/lib/apt/lists/*

ENV DISPLAY=:99
