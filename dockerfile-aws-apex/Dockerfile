FROM alpine:3.7

RUN apk add --update jq curl python py-pip make bash \
  libc6-compat python-dev gcc musl-dev libffi-dev openssl-dev git
RUN curl https://raw.githubusercontent.com/apex/apex/master/install.sh | sh
RUN apex upgrade
RUN pip install --upgrade pip
RUN pip install awscli
RUN pip install awscurl