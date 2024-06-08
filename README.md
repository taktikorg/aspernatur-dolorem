# @taktikorg/aspernatur-dolorem <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Set? This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isSet = require('@taktikorg/aspernatur-dolorem');
assert(!isSet(function () {}));
assert(!isSet(null));
assert(!isSet(function* () { yield 42; return Infinity; });
assert(!isSet(Symbol('foo')));
assert(!isSet(1n));
assert(!isSet(Object(1n)));

assert(!isSet(new Map()));
assert(!isSet(new WeakSet()));
assert(!isSet(new WeakMap()));

assert(isSet(new Set()));

class MySet extends Set {}
assert(isSet(new MySet()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@taktikorg/aspernatur-dolorem
[npm-version-svg]: https://versionbadg.es/inspect-js/@taktikorg/aspernatur-dolorem.svg
[deps-svg]: https://david-dm.org/inspect-js/@taktikorg/aspernatur-dolorem.svg
[deps-url]: https://david-dm.org/inspect-js/@taktikorg/aspernatur-dolorem
[dev-deps-svg]: https://david-dm.org/inspect-js/@taktikorg/aspernatur-dolorem/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@taktikorg/aspernatur-dolorem#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@taktikorg/aspernatur-dolorem.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@taktikorg/aspernatur-dolorem.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@taktikorg/aspernatur-dolorem.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@taktikorg/aspernatur-dolorem
[codecov-image]: https://codecov.io/gh/inspect-js/@taktikorg/aspernatur-dolorem/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@taktikorg/aspernatur-dolorem/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@taktikorg/aspernatur-dolorem
[actions-url]: https://github.com/taktikorg/aspernatur-dolorem/actions
