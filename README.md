Heroku buildpack: Apache
=================================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for vendoring Apache Httpd into your project. It doesn't do anything else, so to actually compile your app you should use [heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi) to combine it with a real buildpack.


Usage
-----

    $ ls
    .buildpacks

    $ heroku create --stack cedar --buildpack http://github.com/dollar/heroku-buildpack-multi.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    ...