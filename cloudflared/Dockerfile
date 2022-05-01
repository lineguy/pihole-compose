FROM alpine:3.15

ENV version="2022.4.1"

RUN apk update \
  && apk add wget bind-tools

RUN wget https://github.com/cloudflare/cloudflared/releases/download/${version}/cloudflared-linux-arm \
  && mv ./cloudflared-linux-arm /usr/local/bin/cloudflared

RUN chmod +x /usr/local/bin/cloudflared
ENTRYPOINT [ "/usr/local/bin/cloudflared" ]
