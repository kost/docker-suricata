FROM debian:latest
MAINTAINER kost - https://github.com/kost

RUN apt-get -qq update && \
apt-get install -yq suricata && \
rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN mkdir /work
VOLUME ["/work"]
WORKDIR /work

ENTRYPOINT ["suricata"]
CMD ["--help"]


