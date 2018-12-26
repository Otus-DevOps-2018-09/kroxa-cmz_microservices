FROM ruby:2.2

ENV APP_HOME=/app POST_SERVICE_HOST=post POST_SERVICE_PORT=5000 COMMENT_SERVICE_HOST=comment COMMENT_SERVICE_PORT=9292

WORKDIR $APP_HOME

ADD . $APP_HOME

RUN apt-get update -qq && apt-get install -y build-essential && \
    bundle install 


CMD ["puma"]
