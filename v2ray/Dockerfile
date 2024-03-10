FROM alpine:3.16
RUN apk add v2ray
COPY ./config.json /config.json
ENV V2RAY_VMESS_AEAD_FORCED=false
EXPOSE 80 9007 9008 9009

CMD ["/usr/bin/v2ray","run", "-c", "config.json"]
