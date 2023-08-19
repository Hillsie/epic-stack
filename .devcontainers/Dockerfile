FROM mcr.microsoft.com/devcontainers/typescript-node:1-20-bullseye as base

# Upate the base image versions
RUN apt-get update \
    && apt-get -y install --no-install-recommends \
    && apt-get install openssl -y \
# Cleanup updates
    && apt-get autoremove -y \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /usr/src/app
