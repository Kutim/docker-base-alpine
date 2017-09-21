FROM alpine:3.1

LABEL maintainer "1252900197@qq.com"

# 定义环境变量
ENV TIME_ZONE Asia/Shanghai

RUN echo "http://mirrors.ustc.edu.cn/alpine/v3.1/main/" > /etc/apk/repositories \
    && apk update \
    && apk add tzdata \
    && echo "${TIME_ZONE}" > /etc/timezone \
    && ln -sf /usr/share/zoneinfo/${TIME_ZONE} /etc/localtime

