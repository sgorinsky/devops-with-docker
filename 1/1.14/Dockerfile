FROM ruby:latest

RUN gem install bundler

COPY . .
RUN cd rails-example-app && bundle install
RUN rails db:migrate

CMD ["rails", "s"]
