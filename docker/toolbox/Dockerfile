FROM alpine:3.6

RUN apk update && \
    apk add bash bash-completion bash-doc tar bind-tools curl jq && \
    rm -rf /tmp/* /var/cache/apk/*

COPY entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh


ENTRYPOINT [ "/entrypoint.sh" ]
