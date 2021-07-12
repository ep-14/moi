FROM ubuntu

ENV TZ Asia/Tokyo
ENV APP_NAME /kafka

WORKDIR $APP_NAME

RUN apt-get update && apt-get install -y --no-install-recommends \
    openjdk-8-jdk \
    sudo \
    curl \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* \
    && curl -sL https://downloads.apache.org/kafka/2.8.0/kafka_2.13-2.8.0.tgz \
    | tar -xz --strip=1

