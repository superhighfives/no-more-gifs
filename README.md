# No More Gifs

A celebration of the static image. It's a one-page joke site: the words "No More Gifs" over a looping, full-screen YouTube video. Viva la no more gifs!

Status: archived. Made in January 2013 and hosted on Heroku. It's no longer online.

## Running it

```sh
bundle
bundle exec foreman start
```

The Gemfile is from 2013 and doesn't pin versions, so it will need some work to install on a current Ruby.

## How it works

- `app.rb` is a Sinatra app that renders `views/index.haml`.
- It compiles the Sass in `views/stylesheets` (with Compass) and the CoffeeScript in `views/javascripts` on each request.
