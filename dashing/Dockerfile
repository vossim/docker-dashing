FROM vossim/base-images:jessie

RUN apt-get update \
  && apt-get upgrade -y \
  && apt-get install -y gem bundler nodejs \
  && gem install dashing \
  && cd /opt/ \
  && dashing new dashboard \
  && cd dashboard \
  && bundle
CMD cd /opt/dashboard && dashing start
