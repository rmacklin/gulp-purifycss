# @rmacklin/gulp-purifycss

This is a fork of [`gulp-purifycss`](https://github.com/purifycss/gulp-purifycss)
which includes the changes from
[PR #24](https://github.com/purifycss/gulp-purifycss/pull/24) to remove the
dependency on the deprecated `gulp-util` package.

The original README follows.

# gulp-purifycss

Clean unnecessary CSS with [PurifyCSS](https://github.com/purifycss/purifycss)

## Information

<table>
<tr>
<td>Package</td><td>gulp-purifycss</td>
</tr>
<tr>
<td>Description</td>
<td>Clean unnecessary CSS</td>
</tr>
<tr>
<td>Node Version</td>
<td>>= 0.10</td>
</tr>
</table>

## Usage

```js
var purify = require('gulp-purifycss');

gulp.task('css', function() {
  return gulp.src('./public/app/example.css')
    .pipe(purify(['./public/app/**/*.js', './public/**/*.html']))
    .pipe(gulp.dest('./dist/'));
});
```
