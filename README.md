# Lektor-bootstrap-portfolio

Simple portfolio theme for [Lektor](https://www.getlektor.com) with [Bootstrap](http://getbootstrap.com/) based on the [portfolio guide from Lektor documentation](https://www.getlektor.com/docs/guides/portfolio/) with support for google analytics, including some funky CSS patterns.


See the [demo](https://www.datamaplab.com/projects)

## Getting started

If you don't have Lektor installed yet, follow the instructions from the official doc [here](https://www.getlektor.com/downloads/).

After cloning the repository, install the dependencies (like bootstrap). You need to have [npm](https://github.com/npm/npm) installed.


	cd webpack
	npm install

Launch the development server

	lektor server -f webpack

You can now edit your portfolio at `http://127.0.0.1:5000`


## Configuration in production

Copy the file `webpack/config/default.js` to `webpack/config/prod.js`, edit the google analytics tracking ID, then build with:


	TARGET=prod lektor build -f webpack


## Selecting the base style

The projects imports the themes from [Bootswatch](http://bootswatch.com/). You can select the one to be used in `webpack/js/main.js`.






