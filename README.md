# gulp-node-inspector

A gulp node-inspector wrapper

Perfect for development.

## Installation

`npm install gulp-node-inspector --save-dev`

## Usage

```javascript
// Gulpfile.js
var gulp = require('gulp');
var nodeInspector = require('gulp-node-inspector');

gulp.task('debug', function () {
  return nodeInspector({
    'web-port': 8081,
    'web-host': 'localhost',
    'debug-port': 5082,
    'save-live-edit': false,
    preload: false,
    'stack-trace-limit': 4
  });
});
```

It works well with [gulp-nodemon](https://github.com/JacksonGariety/gulp-nodemon)

## Options

You can pass an object to `nodeInspector` with options [specified in node-inspector config](https://github.com/node-inspector/node-inspector#options).