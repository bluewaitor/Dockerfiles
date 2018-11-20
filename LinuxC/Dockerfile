FROM alpine:3.8
LABEL maintainer="bluewaitor"
RUN apk update && \
    apk add --no-cache \
    build-base \
    && rm -rf /var/cache/apk/*
WORKDIR /code
ENTRYPOINT [ "gcc" ]
CMD [ "-v" ]