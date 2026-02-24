FROM ghcr.io/ptero-eggs/yolks:python_3.11
USER root
RUN apt-get update \
    && apt-get install -y openjdk-21-jre-headless \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
USER container
