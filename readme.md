# query-dom [![Build Status](https://travis-ci.org/micnews/query-dom.png?branch=master)](https://travis-ci.org/micnews/query-dom)

query-focused &amp; somewhat standards compliant subset of the DOM

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install query-dom --save
```

## Usage

```js
import queryDom from 'query-dom';

const elm = queryDom('<div><foo style="font-size: 12px" class="bar"></foo></div>')[0];
const child = elm.getElementsByTagName('foo')[0];

console.log(child.style.fontSize);
console.log(child.classList.contains('bar'), child.classList.contains('bas'));

```

## Tests

```sh
npm install
npm test
```

## Dependencies

- [camelcase-css](https://github.com/stevenvachon/camelcase-css): Convert a dash-separated CSS property to a camelCased DOM property.
- [es6-set](https://github.com/medikoo/es6-set): ECMAScript6 Set polyfill
- [object-assign](https://github.com/sindresorhus/object-assign): ES6 Object.assign() ponyfill
- [parse5](https://github.com/inikulin/parse5): WHATWG HTML5 specification-compliant, fast and ready for production HTML parsing/serialization toolset for Node.js
- [to-fast-properties](https://github.com/sindresorhus/to-fast-properties): Force V8 to use fast properties for an object

## Dev Dependencies

- [ava](https://github.com/sindresorhus/ava): Futuristic test runner 🚀
- [babel-cli](https://github.com/babel/babel/tree/master/packages): Babel command line.
- [babel-core](https://github.com/babel/babel/tree/master/packages): Babel compiler core.
- [babel-preset-es2015](https://github.com/babel/babel/tree/master/packages): Babel preset for all es2015 plugins.
- [devtool](https://github.com/Jam3/devtool): runs Node.js programs through Chromium DevTools
- [jsdom](https://github.com/tmpvar/jsdom): A JavaScript implementation of the DOM and HTML standards
- [minidom](https://github.com/montagejs/minidom): Small DOM level 1 implementation
- [npm-run-all](https://github.com/mysticatea/npm-run-all): A CLI tool to run multiple npm-scripts in parallel or sequential.
- [nyc](https://github.com/bcoe/nyc): a code coverage tool that works well with subprocesses.
- [package-json-to-readme](https://github.com/zeke/package-json-to-readme): Generate a README.md from package.json contents
- [semistandard](https://github.com/Flet/semistandard): All the goodness of `feross/standard` with semicolons sprinkled on top.
- [snazzy](https://github.com/feross/snazzy): Format JavaScript Standard Style as Stylish (i.e. snazzy) output
- [tsml](https://github.com/rvagg/tsml): ES6 template string tag for multi-line cleaning - squash multi-line strings into a single line


## License

MIT

_Generated by [package-json-to-readme](https://github.com/zeke/package-json-to-readme)_
