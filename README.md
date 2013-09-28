# Blank Seed App

Originally setup by [Brian Ford](http://briantford.com/blog/angular-express.html). Forked to add 
support for [Bootstrap 3.0](http://getbootstrap.com/), [Animate.css](http://daneden.me/animate/) and 
[Google SPDY](https://github.com/indutny/node-spdy) dependencies. NOTE: SPDY requires SSL 
(i.e. https://localhost:3000/) and I've provided example keys which are used for testing. In 
production, you'll want to generate more authoritative keys :) 

Start an awesome app with AngularJS on the front, Express + Node on the back. This project is an
application skeleton for a typical [AngularJS](http://angularjs.org/) web app for those who want
to use Node to serve their app.

The seed contains angular libraries, test libraries and a bunch of scripts all preconfigured for
instant web development gratification. Just clone the repo (or download the zip/tarball) and
you're ready to develop your application. 

The seed app shows how to wire together Angular client-side components with Express on the server.
It also illustrates writing angular partials/views with the Jade templating library.

_Note: Although Jade supports interpolation, you should be doing that mostly on the client. Mixing
server and browser templating will convolute your app. Instead, use Jade as a syntactic sugar for
HTML, and let AngularJS take care of interpolation on the browser side._

## How to use angular-express-seed

Clone the angular-express-seed repository, run `npm install` to grab the dependencies, and start hacking!

### Running the app

Runs like a typical express app:

    node app.js

### Running tests

Coming soon!

### Receiving updates from upstream

Just fetch the changes and merge them into your project with git.


## Directory Layout 
    
    app.js              	--> app config
    keys/					--> example (required) SSL keys for use with SPDY
    node_modules/			--> run 'npm install' to download these
    package.json    		--> for npm
    public/             	--> all of the files to be used in on the client side
      css/              	--> css files
        app.css         	--> default stylesheet
        animate.min.css		-->	animating div elements (http://daneden.me/animate/)
        bootstrap.min.css	--> responsive ui layouts (http://getbootstrap.com/)
      img/              	--> image files
      js/               	--> javascript files
        app.js          	--> declare top-level app module
        controllers.js  	--> application controllers
        directives.js   	--> custom angular directives
        filters.js      	--> custom angular filters
        services.js     	--> custom angular services
        lib/            	--> angular and 3rd party JavaScript libraries
          angular/
            angular.js            --> the latest angular js
            angular.min.js        --> the latest minified angular js
            angular-*.js          --> angular add-on modules
            version.txt           --> version number
    routes/
      api.js            --> route for serving JSON
      index.js          --> route for serving HTML pages and partials
    views/
      index.jade        --> main page for app
      layout.jade       --> doctype, title, head boilerplate
      partials/         --> angular view partials (partial jade templates)
        partial1.jade
        partial2.jade



## Example App 

A simple [blog](https://github.com/btford/angular-express-blog) based on this seed.


## Contact 

For more information on AngularJS please check out http://angularjs.org/
For more on Express and Jade, http://expressjs.com/ and http://jade-lang.com/ are
your friends.

## License
MIT 
