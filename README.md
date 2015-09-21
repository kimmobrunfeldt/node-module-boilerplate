# Node module boilerplate

[![Build Status](https://travis-ci.org/kimmobrunfeldt/repo.svg?branch=master)](https://travis-ci.org/kimmobrunfeldt/repo)

Features:

* [Automated releasing](CONTRIBUTING.md#release) / version bumping
* Mocha tests
* Linters
* Travis integration

Get started

* [ ] `curl -fsSL https://github.com/kimmobrunfeldt/node-module-boilerplate/archive/master.tar.gz | tar -xzvv`
* [ ] `mv node-module-boilerplate-master <module>`
* [ ] [Setup package.json](#setup-package-json)
* [ ] Check CONTRIBUTING.md
* [ ] Check LICENSE
* [ ] Check .travis.yml
* [ ] Write tests
* [ ] Write functionality
* [ ] Check README.md and write documentation
* [ ] [Release](CONTRIBUTING.md#release). Bump to 1.0.0 as soon as possible, it makes versions more useful.

## Structure explained

* `src` Module source code. Helps to separate the actual module code from assisting files like `package.json`.
* `test` Tests.
* `tools` Tools for developers who work with the project.

## Setup package.json

Run:

```bash
npm init
npm install --save-dev mocha eslint jscs releasor
```

Set main:
```json
{
  "main": "src/index.js"
}
```

NPM scripts:

```json
{
  "scripts": {
    "start": "node ./src/index.js",
    "ci": "./tools/ci.sh",
    "test": "mocha",
    "eslint": "eslint --ext .js ./src ./test",
    "jscs": "jscs ./src ./test"
  }
}
```

Few useful paragraphs for new projects, fill those:

## How it works

TODO: fill

## Install

```
npm install module
```

## Usage

TODO: fill

## License

MIT
