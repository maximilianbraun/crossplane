FROM --platform=$BUILDPLATFORM alpine:3.19

ARG TARGETOS
ARG TARGETARCH

RUN apk add --no-cache \
    docker-cli

COPY bin/${TARGETOS}_${TARGETARCH}/crank /usr/local/bin/crossplane
WORKDIR /crossplane

ENTRYPOINT ["/usr/local/bin/crossplane"]