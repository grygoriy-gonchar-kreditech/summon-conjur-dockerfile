FROM openjdk:8-jre-alpine

RUN apk update \
    && apk add bash tar curl wget

RUN curl -sSL https://raw.githubusercontent.com/ggonchar/summon/master/install.sh | bash \
    && mkdir /usr/local/lib/summon \
    && curl -sSL https://github.com/conjurinc/summon-conjur/releases/download/v0.2.0/summon-conjur_v0.2.0_linux-amd64.tar.gz | tar xvz -C /usr/local/lib/summon
