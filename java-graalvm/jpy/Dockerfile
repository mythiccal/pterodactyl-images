FROM ghcr.io/ptero-eggs/yolks:python_3.11
USER root
RUN apt-get update \
    && apt-get install -y wget apt-transport-https ca-certificates gnupg \
    && wget -qO - https://packages.adoptium.net/artifactory/api/gpg/key/public | gpg --dearmor -o /etc/apt/trusted.gpg.d/adoptium.gpg \
    && echo "deb https://packages.adoptium.net/artifactory/deb $(awk -F= '/^VERSION_CODENAME/{print$2}' /etc/os-release) main" > /etc/apt/sources.list.d/adoptium.list \
    && apt-get update \
    && apt-get install -y temurin-21-jre \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
USER container
