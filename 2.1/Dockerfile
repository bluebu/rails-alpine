FROM ruby:2.1-alpine
MAINTAINER bluebu <bluebuwang@gmail.com>

ENV RAILS_VERSION="4.2.6" \
    BUILD_PACKAGES="curl-dev build-base" \
    DEV_PACKAGES="tzdata libxml2 libxml2-dev libxslt libxslt-dev mysql-client imagemagick" 

RUN \
  apk --update --upgrade add $BUILD_PACKAGES $DEV_PACKAGES

RUN \
  gem install -N nokogiri -- --use-system-libraries && \
  gem install -N rails --version "$RAILS_VERSION" && \
  echo 'gem: --no-document' >> ~/.gemrc && \
  cp ~/.gemrc /etc/gemrc && \
  chmod uog+r /etc/gemrc && \

  # cleanup and settings
  bundle config --global build.nokogiri  "--use-system-libraries" && \
  bundle config --global build.nokogumbo "--use-system-libraries" && \
  rm -rf /usr/lib/lib/ruby/gems/*/cache/* && \
  rm -rf ~/.gem

CMD [ "irb" ]
