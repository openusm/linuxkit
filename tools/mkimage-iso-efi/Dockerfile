FROM linuxkit/alpine:34af9cb1990debd17fae6d4198c62ce3910d9908

RUN \
  apk update && apk upgrade && \
  apk add --no-cache \
  dosfstools \
  libarchive-tools \
  binutils \
  gummiboot \
  mtools \
  xorriso \
  && true

COPY . .

ENTRYPOINT [ "/make-efi" ]
