# @zitterorg/velit-autem <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

For use with React PropTypes. Will error on any prop not explicitly specified.

## Usage

```jsx
import PropTypes from 'prop-types';
import exact from '@zitterorg/velit-autem';

function Foo({ foo, bar }) {
  return <div>{foo}{bar}</div>
}
Foo.propTypes = exact({
  foo: PropTypes.string,
  bar: PropTypes.number,
});

<Foo foo="hi" bar={3} /> // no warnings

<Foo foo="hi" bar={3} baz="extra" /> // propTypes warning!
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@zitterorg/velit-autem
[npm-version-svg]: http://versionbadg.es/ljharb/@zitterorg/velit-autem.svg
[deps-svg]: https://david-dm.org/ljharb/@zitterorg/velit-autem.svg
[deps-url]: https://david-dm.org/ljharb/@zitterorg/velit-autem
[dev-deps-svg]: https://david-dm.org/ljharb/@zitterorg/velit-autem/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@zitterorg/velit-autem#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@zitterorg/velit-autem.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@zitterorg/velit-autem.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@zitterorg/velit-autem.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@zitterorg/velit-autem
[codecov-image]: https://codecov.io/gh/ljharb/@zitterorg/velit-autem/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@zitterorg/velit-autem/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@zitterorg/velit-autem
[actions-url]: https://github.com/zitterorg/velit-autem/actions
