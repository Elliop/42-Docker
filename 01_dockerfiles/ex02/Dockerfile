FROM ruby

ONBUILD RUN apt-get update && apt-get upgrade -y && apt-get install nodejs -y
ONBUILD RUN gem install rails
ONBUILD WORKDIR /opt
ONBUILD RUN rails new app
ONBUILD WORKDIR app
ONBUILD RUN bundle install
