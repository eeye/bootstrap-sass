# Bootstrap for Sass

Forked from https://github.com/twbs/bootstrap-sass/tree/v3.3.7

## Changelog

- added new grid breakpoint at 576px (Medium Small)
	- valid from 576px to 767px
	- new order xs -> ms -> sm ...
	- the short cut ist **ms**
	- usage e.g. **col-ms-6**, **hidden-ms** etc.

##Usage

Create bootstrap.min.scss file with the following imports
``` 
// create icons (glyphicon)
$icon-font-path: "assets/fonts/bootstrap/";
@import "assets/stylesheets/bootstrap-sprockets";
// bootstrap for itself
@import "assets/stylesheets/bootstrap";
```
Run sass to compile .css file, e.g.
```
sass --watch --unix-newlines bootstrap.min.scss:bootstrap.min.css --style compressed
```