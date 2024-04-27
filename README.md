# @omegion1npm/modi-repudiandae-mollitia <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Simple ES6 [Array.prototype.find](http://people.mozilla.org/%7Ejorendorff/es6-draft.html#sec-@omegion1npm/modi-repudiandae-mollitia) polyfill for older environments taken from [es6-shim](https://github.com/paulmillr/es6-shim).

For browsers and node.js.

## Installation
* Just include repo before your scripts.
* `npm install @omegion1npm/modi-repudiandae-mollitia`

## Usage

* `Array.prototype.find(predicate[, thisArg])` returns first item that matches `predicate` function.
* `predicate(value, index, collection)`: takes three arguments
    * `value`: current collection element
    * `index`: current collection element index
    * `collection`: the collection

```javascript
// as a function
var find = require('@omegion1npm/modi-repudiandae-mollitia');
find([1, 2], function (x) { return x === 2; }); // 2

// to shim it
require('@omegion1npm/modi-repudiandae-mollitia').shim();
```

Code example:

```javascript
// Default:
[1, 5, 10, 15].find(function (a) { return a > 9; }) // 10
```

## Acknowledgements

Tests, fixes, and travis support added by [_duncanhall](http://twitter.com/_duncanhall)

## License

[The MIT License](https://github.com/paulmillr/mit) (c) 2016 Paul Miller (http://paulmillr.com)

[package-url]: https://npmjs.org/package/@omegion1npm/modi-repudiandae-mollitia
[npm-version-svg]: https://versionbadg.es/es-shims/Array.prototype.find.svg
[deps-svg]: https://david-dm.org/es-shims/Array.prototype.find.svg
[deps-url]: https://david-dm.org/es-shims/Array.prototype.find
[dev-deps-svg]: https://david-dm.org/es-shims/Array.prototype.find/dev-status.svg
[dev-deps-url]: https://david-dm.org/es-shims/Array.prototype.find#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@omegion1npm/modi-repudiandae-mollitia.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@omegion1npm/modi-repudiandae-mollitia.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@omegion1npm/modi-repudiandae-mollitia.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@omegion1npm/modi-repudiandae-mollitia
[codecov-image]: https://codecov.io/gh/es-shims/Array.prototype.find/branch/master/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/es-shims/Array.prototype.find/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/es-shims/Array.prototype.find
[actions-url]: https://github.com/es-shims/Array.prototype.find/actions
