ARG VARIANT=bullseye
ARG VERSION=3.12
FROM mcr.microsoft.com/devcontainers/python:${VERSION}-${VARIANT}

RUN export DEBIAN_FRONTEND=noninteractive \
    && apt-get update \
    && apt-get install -y xdg-utils \
    && curl -fsSL https://aka.ms/install-azd.sh | bash \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*