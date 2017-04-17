# api documentation for  [papaparse (v4.2.0)](http://papaparse.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-papaparse.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-papaparse) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-papaparse.svg)](https://travis-ci.org/npmdoc/node-npmdoc-papaparse)
#### Fast and powerful CSV parser for the browser that supports web workers and streaming large files. Converts CSV to JSON and JSON to CSV.

[![NPM](https://nodei.co/npm/papaparse.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/papaparse)

- [https://npmdoc.github.io/node-npmdoc-papaparse/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-papaparse/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-papaparse/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-papaparse/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-papaparse/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-papaparse/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matthew Holt",
        "url": "https://twitter.com/mholt6"
    },
    "bugs": {
        "url": "https://github.com/mholt/PapaParse/issues"
    },
    "dependencies": {},
    "description": "Fast and powerful CSV parser for the browser that supports web workers and streaming large files. Converts CSV to JSON and JSON to CSV.",
    "devDependencies": {
        "chai": "^3.0.0",
        "connect": "^3.3.3",
        "grunt": "^0.4.5",
        "grunt-contrib-uglify": "^0.6.0",
        "mocha": "^2.2.5",
        "mocha-phantomjs": "^3.5.4",
        "open": "0.0.5",
        "phantomjs": "1.9.1 - 1.9.7-15",
        "serve-static": "^1.7.1"
    },
    "directories": {},
    "dist": {
        "shasum": "ac5bed7de39445dabb6616a507024b8b88eee7c3",
        "tarball": "https://registry.npmjs.org/papaparse/-/papaparse-4.2.0.tgz"
    },
    "gitHead": "fd6431e385468ef3c1c64f7ccb4c47c435631e25",
    "homepage": "http://papaparse.com",
    "keywords": [
        "csv",
        "parser",
        "parse",
        "parsing",
        "delimited",
        "text",
        "data",
        "auto-detect",
        "comma",
        "tab",
        "pipe",
        "file",
        "filereader",
        "stream",
        "worker",
        "workers",
        "thread",
        "threading",
        "multi-threaded",
        "jquery-plugin"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "http://opensource.org/licenses/MIT"
        }
    ],
    "main": "papaparse.js",
    "maintainers": [
        {
            "name": "mholt"
        },
        {
            "name": "pokoli"
        }
    ],
    "name": "papaparse",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mholt/PapaParse.git"
    },
    "scripts": {
        "test": "npm run test-node && npm run test-phantomjs",
        "test-browser": "node tests/test.js",
        "test-node": "mocha tests/node-tests.js tests/test-cases.js",
        "test-phantomjs": "node tests/test.js --phantomjs"
    },
    "version": "4.2.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
