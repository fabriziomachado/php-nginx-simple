# How to setup Heroku Buildpack for PHP with Nginx

This will set up a fresh WordPress install on Heroku with the newly released [Heroku Buildpack for PHP](https://github.com/heroku/heroku-buildpack-php).

* `nginx` - Nginx for serving web content.
* `PHP` - PHP-FPM for process management

# Getting started

Use the Deploy to Heroku button, or use the old fashioned way described below.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

# Clone this repository into a new directory.

1) Create your Heroku app.
2) Create project in Heroku

* Note: Change `name-project-here` for your name project

```bash
heroku apps:create name-project-here --stack cedar --buildpack https://github.com/heroku/heroku-buildpack-php --region us
```

3) Define your Global variables

```bash
heroku config:set SITE_TITLE=hola Mundo
```

4) Deploy your site to Heroku.

```bash
git add .
git commit -am "Initial commit"
git push heroku master
```

5) Finish
```bash
heroku open
```

# Overview

```
└── public
```

