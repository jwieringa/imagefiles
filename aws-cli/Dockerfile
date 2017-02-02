# docker run -it \
#   -e AWS_ACCESS_KEY_ID=secret \
#   -e AWS_SECRET_ACCESS_KEY=secret \
#   -e AWS_DEFAULT_REGION=us-east-1 \
#   aws-cli aws

FROM alpine:3.5

RUN apk add --update \
      ca-certificates \
      python3 \
      py-pip \
      && rm -rf /var/cache/apk/*

RUN mkdir -p /tmp/build \
      && pip install awscli \
      && rm -rf /tmp/build
