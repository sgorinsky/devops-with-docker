FROM ruby:2.6.0

RUN apt-get update -y && apt-get install nodejs -y

COPY . .
WORKDIR rails-example-project

RUN gem install bundler:1.17.2
RUN bundler install

RUN rails db:migrate

EXPOSE 3000
CMD ["rails", "s"]
