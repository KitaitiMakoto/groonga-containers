FROM debian:jessie
MAINTAINER KITAITI Makoto

COPY groonga.list /etc/apt/sources.list.d/
RUN apt-get update && \
    apt-get upgrade && \
    apt-get install -y --allow-unauthenticated groonga-keyring && \
    apt-get update && \
    apt-get install -y groonga groonga-tokenizer-mecab groonga-token-filter-stem && \
    apt-get clean
