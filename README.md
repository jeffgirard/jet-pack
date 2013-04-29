# jet-pack

A boilerplate Sinatra app set up with:

- Slim, Haml, ERB and Markdown
- Sass/Compass
- CoffeeScript
- Foreman
- Rack-livereload

## Initialize

```
git clone git://github.com/raul/jet-pack.git your-project
cd your-project
rm -rf .git
bundle install
git init .
git commit -a -m"jet-pack boilerplate"
```

## Develop

Start your app with `foreman start` and you're up and flying at [localhost:5000](http://localhost:5000) (you can select a different port by setting a `$PORT` env. var).

Views:

- `/views/layout.slim` will be rendered for all your views
- `/views/foo/bar.md`, `/views/foo/bar.erb`, `/views/foo/bar.slim` or `/views/foo/bar.haml` will be served under `/foo/bar`

Assets:

- `/public/coffee/foo.coffee` will be served under `/js/foo.js`
- `/public/sass/foo.sass` will be served under `/css/foo.css`

While working locally, the browser will automatically reload the page whenever you modify a source file – quite handy for quick previews.

## Deploy to Heroku

```
heroku create your-app-name
git push heroku master
```

Heroku won't install `livereload` – you won't need it on production.

## Thanks

This project was heavily inspired by [loafer](https://github.com/zeke/loafer), another cool project by the charming and talented [Zeke](https://twitter.com/zeke).

## License

jet-pack doesn't have a license: it just stands on the shoulders of giants.