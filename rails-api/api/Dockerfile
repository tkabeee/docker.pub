# syntax=docker/dockerfile:1
FROM ruby:3
RUN apt-get update -qqy && apt-get install -qqy \
    sudo \
    vim \
    wget \
    lsof \
    build-essential \
    libc6-dev \
    mariadb-client \
    nodejs \
    yarn

ENV APP_HOME=/app

WORKDIR $APP_HOME

# Add a script to be executed every time the container starts.
COPY ./entrypoint.sh /usr/bin/
RUN chmod +x /usr/bin/entrypoint.sh
ENTRYPOINT ["entrypoint.sh"]
EXPOSE 3000

# Configure the main process to run when running the image
CMD ["rails", "server", "-b", "0.0.0.0"]
