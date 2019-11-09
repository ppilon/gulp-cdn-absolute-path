gulp-replace-assets-path
=============

> A gulp plugin for replacing local path with a cdn path

This repository was forked from https://github.com/anhulife/gulp-cdn-absolute-path

## Install

```
npm install --save-dev gulp-replace-assets-path
```

## Examples
```js
var gulp = require('gulp');
var cdnAbsolutePath = require('gulp-replace-assets-path');

gulp.task('cdn-absolute-path', function () {
	gulp.src('template/**/*.html')
		.pipe(cdnAbsolutePath({asset: 'static', cdn: 'http://www.a.com'}))
		.pipe(gulp.dest('template'));
});
```