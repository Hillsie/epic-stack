FROM mcr.microsoft.com/devcontainers/typescript-node:1-20-bullseye as base
# Microsoft Dev Containers 
# 1. Install docker desktop and docker requirements
# 2. Install MS Remote explorer
# 3. In Microsoft Remote Explorer, add new dev container from github
# https://code.visualstudio.com/docs/devcontainers/containers
# https://marketplace.visualstudio.com/items?itemName=ms-vscode.remote-explorer 
# Upate the base image versions
RUN apt-get update \
    && apt-get -y install --no-install-recommends \
    && apt-get install openssl -y \
# Cleanup updates
    && apt-get autoremove -y \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /usr/src/app
