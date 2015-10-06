# Materializer
Frontend coding environment

Building static websites and interfaces is sometimes a tedious task if we use just plain HTML and CSS, and as we know those languages are not very scalable and maintainable, so here's a frontend coding environment that comes in handy. With Materializer you can take the advantages of more versatile languages like Sass and Jade to make static website development efficient and as painless as possible.

Materializer also features a local web-server and some neat features, read on for more information.

## Getting Started
To use Materializer you need all the following softwares to be installed on your computer.

 - Node
 - Npm
 - Gulp
 - Bower
 - Git

To get started clone this repo on your local machine:

	git clone https://github.com/pwnjack/materializer.git

Move inside the newly created "materializer" folder and install the default dev-dependencies:

	cd materializer

	npm install

Then install your project's default dependencies (Modernizr, jQuery, MaterializeCSS):

 	bower install

To install more dependencies in your project do it via Bower with the --save option, like so:

 	bower install --save font-awesome


## Usage
Once you have defined all your assets you can start to work on your project, run:

	gulp

This will open up your favorite browser on the project's index page, and while you work on the code it will refresh  the page in real-time to reflect your code's changes (css, js, jade).

To work smoothly Materializer let you build you project using some preprocessors:

- Jade for HTML
- Sass for CSS

Materializer have more nice features:

- Images web-optimization
- CSS autoprefixer
- Code minimization for production
- Bower dependencies injection
- Local preview web-server with BrowserSync

When your project is ready for production, build it:

	gulp build

Your project's optimized version will be stored in the freshly created "dist" folder.

## Helpers
If you want to install an asset later on, stop the server in your terminal (CTRL+C), install the asset via Bower then inject it's reference in your markup:

	gulp inject

Then start the server again:

	gulp serve

And you can get back to work on your code.

If you want to install an asset that is not available on Bower you can do it by copy-pasting it's code in to the following files (depending on code language):

- Javascript into "app/scripts/plugins.js"
- CSS into "app/styles/includes/_plugins.scss"
- For images and fonts you need to add their full path reference into "config.json"

### Feedback
Thanks for reading, your feedback is much appreciated.