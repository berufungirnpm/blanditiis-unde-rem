# @berufungirnpm/blanditiis-unde-rem <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the `byteLength` out of a DataView, robustly.

This will work in node <= 0.10 and < 0.11.4, where there's no prototype accessor, only a nonconfigurable own property.
It will also work in modern engines where `DataView.prototype.byteLength` has been deleted after this module has loaded.

## Example

```js
const dataViewByteLength = require('@berufungirnpm/blanditiis-unde-rem');
const assert = require('assert');

const ab = new ArrayBuffer(42);
const dv = new DataView(ab);
assert.equal(dataViewByteLength(dv), 42);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@berufungirnpm/blanditiis-unde-rem
[npm-version-svg]: https://versionbadg.es/inspect-js/@berufungirnpm/blanditiis-unde-rem.svg
[deps-svg]: https://david-dm.org/inspect-js/@berufungirnpm/blanditiis-unde-rem.svg
[deps-url]: https://david-dm.org/inspect-js/@berufungirnpm/blanditiis-unde-rem
[dev-deps-svg]: https://david-dm.org/inspect-js/@berufungirnpm/blanditiis-unde-rem/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@berufungirnpm/blanditiis-unde-rem#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@berufungirnpm/blanditiis-unde-rem.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@berufungirnpm/blanditiis-unde-rem.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@berufungirnpm/blanditiis-unde-rem.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@berufungirnpm/blanditiis-unde-rem
[codecov-image]: https://codecov.io/gh/inspect-js/@berufungirnpm/blanditiis-unde-rem/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@berufungirnpm/blanditiis-unde-rem/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@berufungirnpm/blanditiis-unde-rem
[actions-url]: https://github.com/inspect-js/@berufungirnpm/blanditiis-unde-rem/actions
