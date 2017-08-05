# README

## 必要なOSパッケージインストール

    $ curl -sL https://deb.nodesource.com/setup_6.x | sudo bash -
    $ curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
    $ echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
    $ sudo apt-get update -qq
    $ sudo apt-get install -y build-essential libmysqlclient-dev nodejs yarn

Docker & Docker Compose

## gems & node modules

    $ bundle install --jobs 4 --retry 5 --path vendor/bundle
    $ yarn

## Start

    $ docker-compose up -d
    $ bundle exec rails s
