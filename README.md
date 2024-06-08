# @patrtorg/est-iure <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the byte length of an ArrayBuffer, even in engines without a `.byteLength` method.

## Example

```js
const assert = require('assert');
const byteLength = require('@patrtorg/est-iure');

assert.equal(byteLength([]), NaN, 'an array is not an ArrayBuffer, yields NaN');

assert.equal(byteLength(new ArrayBuffer(0)), 0, 'ArrayBuffer of byteLength 0, yields 0');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@patrtorg/est-iure
[npm-version-svg]: https://versionbadg.es/inspect-js/@patrtorg/est-iure.svg
[deps-svg]: https://david-dm.org/inspect-js/@patrtorg/est-iure.svg
[deps-url]: https://david-dm.org/inspect-js/@patrtorg/est-iure
[dev-deps-svg]: https://david-dm.org/inspect-js/@patrtorg/est-iure/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@patrtorg/est-iure#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@patrtorg/est-iure.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@patrtorg/est-iure.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@patrtorg/est-iure.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@patrtorg/est-iure
[codecov-image]: https://codecov.io/gh/inspect-js/@patrtorg/est-iure/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@patrtorg/est-iure/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@patrtorg/est-iure
[actions-url]: https://github.com/patrtorg/est-iure/actions
