FROM ruby:2.6.6
ENV LANG C.UTF-8
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs npm && rm -rf /var/lib/apt/lists/*
RUN npm install yarn -g --force
ENV APP_HOME /var/www
RUN mkdir -p $APP_HOME
WORKDIR $APP_HOME
COPY ./docker/rails/Gemfile $APP_HOME/Gemfile
COPY ./docker/rails/Gemfile.lock $APP_HOME/Gemfile.lock
RUN gem install rails
# COPY rails $APP_HOME

# RUN bundle install
