FROM alpine:3.11 as build

ENV HUGO_VERSION=0.69.1

RUN apk add --no-cache curl \
    && curl -sL https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_${HUGO_VERSION}_Linux-64bit.tar.gz | tar xz

FROM alpine:3.11

COPY --from=build /hugo /usr/local/bin

ENTRYPOINT ["hugo"]


