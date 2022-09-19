## for Rails

```bash
docker-compose run --rm api gem install rails
docker-compose run --rm api bundle exec rails new . --force \[options\]
```

options for api

```
--api --database=mysql -M --skip-action-mailbox --skip-action-text --skip-active-job -C -S -J -–skip-hotwire --skip-jbuilder -B
```


Options:

```
-f, --force
-M, --skip-action-mailer
--skip-action-mailbox
--skip-action-text
-O, --skip-active-record
--skip-active-job
--skip-active-storage
-C, --skip-action-cable
-S, --skip-sprockets
-J, --skip-javascript
-–skip-hotwire
--skip-jbuilder
-T, --skip-test
–-skip-system-test
--skip-bootsnap
-B, --skip-bundle
```

Gemfile生成

```
docker-compose run --rm api bundle init
```

gemインストール

```bash
docker-compose run --rm api bundle install
```
