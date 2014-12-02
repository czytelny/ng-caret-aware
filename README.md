Caret aware
===========

AngularJS directive for caret aware elements.

Put it on your HTML input elements and it will track the caret (i.e. cursor) exporting its position in a variable (named after the value assigned to the directive attribute) appended to the parent `$scope`.

Weight: ~1KB.

#### Note

This directive works only as attribute.

Usage
-----

Include AngularJS, the build (e.g., `caretaware.min.js`), and the `leodido.caretAware` AngularJS module.

```html
<input type="text" name="myCursorField" data-caret-aware="cursor"/>
```

Parent scope will contain a `cursor` variable tracking the caret position of input named `myCursorField`.

Or, simply:

```html
<input type="text" name="myCaretField" caret-aware/>
```

Parent scope will contain a `caret` (the default name) variable tracking the caret position of input named `myCaretField`.

#### Note

See [example](/example) directory for furhter details.

Install
-------

To install locally:

```
$ git clone git@github.com:leodido/ng-caret-aware.git
$ cd ng-caret-aware/
$ npm install
```

At the moment this module has not yet been published. Once test suite will be prepared and completed it will be published on online registries.

Build
-----

Build is handled through [Gulp](https://github.com/gulpjs/gulp/) and performed mainly via [Google Closure Compiler](https://github.com/google/closure-compiler).

Need help? Run `gulp help` !

```
# Usage
#   gulp [task]
# 
# Available tasks
#   build                           Build the library 
#    --banner                       Prepend banner to the built file
#    --env=production|development   Kind of build to perform, defaults to production
#   clean                           Clean build directory
#   help                            Display this help text
#   lint                            Lint JS source files
#   version                         Print the library version
```

To build a development version of JS lib:

```
$ gulp build --env dev
```

Or, also:

```
$ npm run development
```

---

[![Analytics](https://ga-beacon.appspot.com/UA-49657176-1/ng-caret-aware)](https://github.com/igrigorik/ga-beacon)
