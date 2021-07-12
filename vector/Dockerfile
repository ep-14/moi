FROM ubuntu

ENV TZ Asia/Tokyo
ENV APP_NAME /vector

WORKDIR $APP_NAME

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    sudo \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* \
    && echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \

