FROM ruby:2.6.0
WORKDIR /app
COPY /rails-example-project /app
EXPOSE 3000
ENV RAILS_ENV=production
ENV RAILS_LOG_TO_STDOUT=true
ENV SECRET_KEY_BASE=antti
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs && gem install bundler -v 1.17.3 && bundle install && npm install yarn -g
RUN rails db:migrate
RUN rake assets:precompile
ENTRYPOINT ["rails", "s", "-e", "production"]