#angular-backtop [![Build Status](https://travis-ci.org/padsbanger/angular-backtop.svg)](https://travis-ci.org/padsbanger/angular-backtop)

A simple *Angular.js* directive to create "Back to top" button when user reaches the end of the page.

You can see a working demo [here](http://padsbanger.github.io/angular-backtop/demo/).

## Installation

Assuming that you already have Angular.js in your app, include *angular-backtop.js* and *angular-backtop.css*.

Add directive as your dependency:

```js
var app = angular.module('app', ['angular.backtop']);
```

Create directive element somewhere inside of your *<body>* tag:

```html
<back-top></back-top>
```

... and thats all, you have a basic button, that will appear when you reach the end of the page. Click on it to be redirected to the top.

## Options

You can pass some more options to the directive.

  - **scroll-speed** - Speed in miliseconds, default value is 600
  - **button-theme** - Themes for button, there is *bootstrap*, *dark* & *light*. Default it *light*.
  - **button-text** - Text, that will be displayed inside of a button. Default is *Scroll top*.


Example:

```html
 <back-top scroll-speed=600 button-theme="light" button-text="Take me back"></back-top>
```

## Tests

```js
npm install
grunt karma:unit
```
