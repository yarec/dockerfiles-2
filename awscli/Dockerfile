FROM jalaziz/base:alpine

RUN  apk add --update python py-pip \
  && pip install awscli \
  && apk del py-pip \
  && rm -rf /var/cache/apk/*

ENTRYPOINT [ "/usr/bin/aws" ]
