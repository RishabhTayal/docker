FROM ruby:2.5-alpine

LABEL "repository"="https://github.com/rishabhtayal/docker"
LABEL "homepage"="https://github.com/rishabhtayal/docker"
LABEL "maintainer"="<Rishabh Tayal> rtayal11@gmail.com"

LABEL "com.github.actions.name"="Danger"
LABEL "com.github.actions.description"="Run Danger"
LABEL "com.github.actions.icon"="alert-triangle"
LABEL "com.github.actions.color"="yellow"

RUN gem install danger

CMD "danger"