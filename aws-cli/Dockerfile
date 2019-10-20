FROM alpine:3.10.2

RUN set -ex \
  \
  && apk --no-cache \
    add \
      bash \
      ca-certificates \
      curl \
      groff \
      jq \
      less \
      python3 \
      py-pip \
  \
  && pip install --no-cache-dir --upgrade pip \
  \
  && pip install --no-cache-dir \
    awscli==1.16.263 \
    s3cmd==2.0.0 \
  \
  && mkdir /root/.aws \
  \
  && aws --version \
  && s3cmd --version
