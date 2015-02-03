# agiles.mx web site

## Local development

First install all the gems

```sh
$ bundle install
```

Running jekyll as a server with auto load enabled

```sh
$ bundle ex jekyll --auto --server
Configuration from /Users/san650/openspace/_config.yml
Auto-regenerating enabled: /Users/san650/openspace -> /Users/san650/openspace/_site
[2014-03-20 21:58:26] INFO  WEBrick 1.3.1
[2014-03-20 21:58:26] INFO  ruby 2.0.0 (2013-06-27) [x86_64-darwin12.5.0]
[2014-03-20 21:58:26] INFO  WEBrick::HTTPServer#start: pid=15593 port=4000
[2014-03-20 21:58:26] regeneration: 1 files changed
[2014-03-20 21:58:26] regeneration: 1 files changed
[2014-03-20 21:58:26] regeneration: 1 files changed
[2014-03-20 21:58:26] regeneration: 1 files changed
[2014-03-20 21:58:26] regeneration: 1 files changed
[2014-03-20 21:58:26] regeneration: 1 files changed
[2014-03-20 21:58:26] regeneration: 1 files changed
[2014-03-20 21:59:33] regeneration: 1 files changed
```

## Deploy to Heroku

### First time

Create a new Heroku application

```sh
$ heroku create MySite
```

Configure the build pack

```sh
$ heroku config:add BUILDPACK_URL=https://github.com/san650/heroku-buildpack-ruby
```

Push the files to Heroku

```sh
$ git push heroku master
```

### Update an installation

Push the changes to Heroku

```sh
$ git push heroku master
```
