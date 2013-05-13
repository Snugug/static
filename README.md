static
======

Static is a static site generation tool utilizing Grunt. It uses [Grunt Generator](https://github.com/clavery/grunt-generator) for HTML generation and [Sass](http://sass-lang.com) and [Compass](http://compass-style.org) for CSS generation. It will minify your PNG, JPG, and SVG images and JSHint and Uglify your JavaScript.

## Static Server

Static will run a server for you to let you develop easily. Simply run `grunt server` to run your server. When running, navigate to `localhost:8000`. If you'd like, you can run `grunt server --launch` to automatically launch the site in your default browser when the server is running

## Static Build

Static will build a out production versions of your files into a `.dist` directory. Run `grunt build` to do so. You can automatically commit your changes to your GitHub depository by running `grunt build --commit`. You can pass a custom commit message in by running `grunt build --commit="Commit Message"`.

## Static Export

If you would like to export your built site to a folder, you can run `grunt export`. This will export your built site to an `export` folder. If you would like to choose where the folder gets exported to, you can run `grunt export --to="path/to/export"`

## Static Deploy

If you're using this to build GitHub pages, you can easily deploy to a `gh-pages` branch in a similar manner to how [Yeoman deploys work](https://github.com/yeoman/yeoman/wiki/Deployment). Make sure this is not in your `gh-pages` branch, and your `gh-pages` branch either doesn't exist, or has only been built using the Deploy command. When you're ready to deploy to `gh-pages`, run `grunt deploy`