FROM alpine:latest
LABEL maintainer="bluewaitor"
RUN apk update && \
    apk add --no-cache  \
    binutils \
    nasm \
    gdb \
    && rm -rf /var/cache/apk/*
WORKDIR /code
ENTRYPOINT [ "nasm" ]
CMD [ "-h" ]