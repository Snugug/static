# static

Static is a static site generation tool utilizing Grunt. It uses [Grunt Generator](https://github.com/clavery/grunt-generator) for HTML generation and [Sass](http://sass-lang.com) and [Compass](http://compass-style.org) for CSS generation. It will also minify your PNG, JPG, and SVG images and JSHint and Uglify your JavaScript. It's equally suited for rapid prototyping, blogging, site creation, really anything you'd like to throw at it. Enjoy!

## Requirements and Installation

In order to run Static, you are going to need to install [Sass+Compass](http://compass-style.org/install/), [Bundler](http://gembundler.com/#getting-started), [Node.js](http://nodejs.org/), [Grunt](http://gruntjs.com/getting-started), and [Bower](http://bower.io/). Once you have all of those installed, run `bundle install` to install the default Compass extensions, `npm install` to install the Node dependencies, and `bower install` to install the Bower components.

## Create

Static will run a server for you to let you develop easily. Simply run `grunt server` to run your server. When running, navigate to `localhost:8000`. If you'd like, you can run `grunt server --launch` to automatically launch the site in your default browser when the server is running

## Build

Static will build a out production versions of your files into a `.dist` directory. Run `grunt build` to do so. You can automatically commit your changes to your GitHub depository by running `grunt build --commit`. You can pass a custom commit message in by running `grunt build --commit="Commit Message"`.

## Export

If you would like to export your built site to a folder, you can run `grunt export`. This will export your built site to an `export` folder. If you would like to choose where the folder gets exported to, you can run `grunt export --to="path/to/export"`

## Deploy

If you're using this to build GitHub pages, you can easily deploy to a `gh-pages` branch in a similar manner to how [Yeoman deploys work](https://github.com/yeoman/yeoman/wiki/Deployment). Make sure this is not in your `gh-pages` branch, and your `gh-pages` branch either doesn't exist, or has only been built using the Deploy command. Make sure that any changes you've made to your Build files have been committed to your repository before deploying, I recommend running `grunt build --commit` before deploying to ensure that everything is there and ready to deploy. When you're ready to deploy to `gh-pages`, run `grunt deploy`. If you're using this to create your User or Organization GitHub page, those are built off of the `master` branch instead of the `gh-pages` branch. Because of this, you are going to need to roll these deploys by hand for the time being.
