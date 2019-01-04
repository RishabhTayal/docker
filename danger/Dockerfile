FROM ruby:2.5-alpine

LABEL "repository"="https://github.com/rishabhtayal/docker"
LABEL "homepage"="https://github.com/rishabhtayal/docker"
LABEL "maintainer"="<Rishabh Tayal> rtayal11@gmail.com"

LABEL "com.github.actions.name"="Danger"
LABEL "com.github.actions.description"="Run Danger"
LABEL "com.github.actions.icon"="alert-triangle"
LABEL "com.github.actions.color"="yellow"

RUN apt-get update -qq && apt-get install -y build-essential p7zip unzip

ENV APP_HOME /myapp
RUN mkdir $APP_HOME
WORKDIR $APP_HOME

ADD ./Gemfile $APP_HOME/Gemfile
ADD Gemfile.lock $APP_HOME/Gemfile.lock

RUN bundle install
CMD bundle exec danger