# Sparkle
Frontend coding environment

## Getting Started
To use Sparkle you need all the following softwares to be installed in your computer.

 - Node
 - Npm
 - Gulp
 - Bower
 - Git

To get started clone this repo on your local machine:

		git clone https://github.com/pwnjack/sparkle.git

Move inside the newly created "sparkle" folder and install the default dev-dependencies:

    npm install

Then install your project's default dependencies (Modernizr, jQuery, MaterializeCSS)

 		bower install

To install more dependencies in your project do it via Bower with the --save option, like so:

 		bower install --save font-awesome


## Usage
Once you have defined all your assets you can start to work on your project, open the project folder in your terminal and run:

		gulp

This will open up your favorite browser on the project's index page, and while you work on the code it will refresh in real-time the browser's page to reflect your code's changes (css, js, jade).

To work smoothly Sparkle let you build you project using some preprocessors:

- Jade for HTML
- Sass for CSS

Sparkle have more nice features:

- Images web-optimization
- Css autoprefixer
- Code minification for production
- Bower dependencies injection
- Preview local web-server with BrowserSync
- Browser real-time updates on code changes

## Helpers
If you want to install an asset later on, stop the server in your terminal, install the asset via Bower then inject it's reference in your markup:

		gulp inject

Then start the server again

		gulp serve

And start to work again on your code.

If you want to install an asset not "bower-ready" you can do it by adding it's full path to the "config.json" file.