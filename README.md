# Pretty-JSONP

This is fork of [jquery-jsonp](https://github.com/jaubourg/jquery-jsonp), but jquery independent.
It`s a compact (1.8kB minified), yet feature-packed solution to implementation of JSONP.

## Licensing

Pretty-JSONP is released under the [MIT license](https://github.com/strayiker/pretty-jsonp/blob/master/MIT-LICENSE.txt).

## Install

npm install --save pretty-jsonp

Note, this implementation uses Object.assign so if u wanna support old browsers u should add a ponyfill like [object-assign](https://github.com/sindresorhus/object-assign).

## Usage

```
import jsonp from 'pretty-jsonp';

jsonp({
  url: 'http://some.cool.domain/api/method',
  data: { param: 'purum' },
  success: () => {},
  error: () => {},
  complete: () => {}
});
```

## Features

features:
* *error recovery* in case of network failure or ill-formed JSON responses,
* precise *control over callback naming* and how it is transmitted in the URL,
* multiple requests with the *same callback name running concurrently*,
* *two caching mechanisms* (browser-based and page based),
* the possibility to *manually abort* the request just like any other AJAX request,
* a *timeout* mechanism.

## Compatibility

Original library has been tested and runs within all major browsers, namely:
* *Internet Explorer 6+*
* *Firefox 2+*
* *Chrome 1+*
* *Safari 3+*
* *Opera 9+*

## Documentation

* [API Documentation](https://github.com/strayiker/pretty-jsonp/blob/master/doc/API.md)
* [Tips & Tricks](https://github.com/strayiker/pretty-jsonp/blob/master/doc/TipsAndTricks.md)
