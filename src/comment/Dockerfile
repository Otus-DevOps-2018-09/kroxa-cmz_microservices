FROM ruby:2.2

ENV APP_HOME=/app COMMENT_DATABASE_HOST=comment_db COMMENT_DATABASE=comments

ADD . $APP_HOME

WORKDIR $APP_HOME

RUN apt-get update -qq && apt-get install -y build-essential && \
    bundle install

CMD ["puma"]
