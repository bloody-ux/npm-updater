npm-updater
---------------

[![NPM version][npm-image]][npm-url]
[![node version][node-image]][node-url]

[npm-image]: https://img.shields.io/npm/v/npm-updater.svg?style=flat-square
[npm-url]: https://npmjs.org/package/npm-updater
[node-image]: https://img.shields.io/badge/node.js-%3E=_0.10-green.svg?style=flat-square
[node-url]: http://nodejs.org/download/

Prompt update of npm package.

## Installation

```bash
$ npm install npm-updater
```

## Usage

```js
var updater = require('npm-updater')

updater({ level: 'major' }).then(execCommands)
```

### Options

- `registry`: support customize registry, default get `publishConfig.registry` from parent package.
- `name`: package name, default get from parent package.
- `version`: pkg version,default get from parent package.
- `tag`: compare with which tag, default to `latest`.
- `abort`: If remote version changed, should we abort? default to `true`.
- `level`: abort level, default to `minor`.
- `interval`: prompt interval, default to `1d`.
- `updateMessage`: appending update message.

## License

MIT
