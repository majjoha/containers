FROM alpine:3.9
MAINTAINER Mathias Jean Johansen <mathias@mjj.io>

RUN apk update && \
    apk upgrade && \
    apk add --no-cache \
    aspell \
    aspell-en \
    biber \
    make \
    texlive-full \
    texmf-dist-fontsextra \
    wget && \
    wget https://github.com/jgm/pandoc/releases/download/2.7.2/pandoc-2.7.2-linux.tar.gz -O pandoc.tar.gz  && \
    tar xvzf pandoc.tar.gz --strip-components 1 -C /usr/local/ && \
    rm pandoc.tar.gz && \
    rm -rf /var/cache/apk/*
