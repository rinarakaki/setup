# Build Session Manager Plugin
FROM --platform=$BUILDPLATFORM golang:1.18-alpine AS ssm-builder

ARG SSM_VERSION=1.2.497.0

RUN set -ex && apk add --no-cache make git gcc libc-dev bash zip
RUN git clone --single-branch --depth 1 -b $SSM_VERSION https://github.com/aws/session-manager-plugin.git
RUN mkdir -p /go/src/github.com && \
    mv session-manager-plugin /go/src/github.com/session-manager-plugin
WORKDIR /go/src/github.com/session-manager-plugin
RUN make release

# Build the final image
FROM --platform=$BUILDPLATFORM alpine:edge

ARG TARGETOS TARGETARCH
COPY --from=ssm-builder /go/src/github.com/session-manager-plugin/bin/${TARGETOS}_${TARGETARCH}_plugin/session-manager-plugin /usr/local/bin/

RUN apk update && apk add --no-cache aws-cli git groff jq socat
