FROM alpine
LABEL maintainer="bluewaitor"
RUN apk update && \
    apk add --no-cache  \
    binutils \
    nasm \
    && rm -rf /var/cache/apk/*
WORKDIR /code
ENTRYPOINT [ "nasm" ]
CMD [ "-h" ]