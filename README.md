# Angular 2 with Webpack
Bare minimum Angular 2 starter template with Webpack (with HTML templates, and LESS). Note this doesn't include any testing libraries, this is just to get you up and going as quickly as possible.

Current Angular version: 2.0.0-rc.1

Includes HTML and LESS loader that will let you compile LESS and also manage importing HTML templates and stylesheets for angular components so you don't need to copy them.

Note you need to use require inside the component when referencing LESS, and HTML files:

    styles: [require('./app.component.less')],
    template: require('./app.component.html')

The path is relative to the component's path. Make sure you use "template" rather than "templateUrl".

## Installation

To get started, simply run:

    npm install

Then to build & run the application (with live reload), use:

    npm run serve

This will build and the app, and run it on http://localhost:8080 by default.

## NPM scripts

Builds with webpack:

    npm run build 

Builds for production (will uglify and minify):

    npm run build:prod
