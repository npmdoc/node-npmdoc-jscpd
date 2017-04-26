# npmdoc-jscpd

#### basic api documentation for  [jscpd (v0.6.11)](https://github.com/kucherenko/jscpd#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-jscpd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jscpd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jscpd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jscpd)

#### Copy/paste detector for programming code, support JavaScript, CoffeeScript, PHP, Ruby, Python, Less, Go, Java, Yaml, C#, C++, C, Puppet, Twig languages

[![NPM](https://nodei.co/npm/jscpd.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jscpd)

- [https://npmdoc.github.io/node-npmdoc-jscpd/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jscpd/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jscpd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jscpd/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jscpd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jscpd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrey Kucherenko",
        "url": "http://kucherenko.org/"
    },
    "bin": {
        "jscpd": "./bin/jscpd"
    },
    "bugs": {
        "url": "https://github.com/kucherenko/jscpd/issues"
    },
    "dependencies": {
        "blamer": "^0.1.9",
        "bluebird": "^3.0.5",
        "cli": ">=0.10.x",
        "cli-table": "^0.3.1",
        "codemirror": ">=4.10.x",
        "colors": "^1.1.2",
        "glob": ">=5.0.x",
        "js-yaml": ">=3.4.x",
        "shelljs": ">=0.5.x",
        "underscore": ">=1.8.x",
        "winston": ">=1.0.x"
    },
    "description": "Copy/paste detector for programming code, support JavaScript, CoffeeScript, PHP, Ruby, Python, Less, Go, Java, Yaml, C#, C++, C, Puppet, Twig languages",
    "devDependencies": {
        "chai": ">=1.10.x",
        "coffee-coverage": ">=0.4.4",
        "coffee-script": ">=1.10.x",
        "coffeelint": "^1.15.0",
        "coveralls": "~2.12.0",
        "istanbul": "^0.4.2",
        "jscpd": ">=0.4.x",
        "mocha": ">=3.x",
        "proxyquire": "^1.7.4",
        "sinon": ">=1.12.x",
        "sinon-chai": "^2.8.0",
        "tv4": "^1.1.4",
        "xml2js": ">=0.4.x"
    },
    "directories": {},
    "dist": {
        "shasum": "3ac3fe808c6e4d7885c5f1fc76c1925f923c79c9",
        "tarball": "https://registry.npmjs.org/jscpd/-/jscpd-0.6.11.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "a52c47358de9d53b0e84917e51ed725f3150ddeb",
    "homepage": "https://github.com/kucherenko/jscpd#readme",
    "keywords": [
        "code",
        "cpd",
        "pmd",
        "analyze",
        "quality",
        "copy",
        "paste",
        "javascript",
        "coffeescript",
        "php",
        "sass",
        "css",
        "python",
        "ruby",
        "java",
        "go",
        "c#",
        "c++",
        "objective-c",
        "c",
        "twig",
        "xml",
        "xsl",
        "html",
        "yaml",
        "swift"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "apk"
        }
    ],
    "name": "jscpd",
    "optionalDependencies": {},
    "preferGlobal": true,
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kucherenko/jscpd.git"
    },
    "scripts": {
        "coverage": "bash scripts/coverage.sh",
        "coveralls": "cat ./coverage/lcov.info | coveralls",
        "jscpd": "jscpd",
        "lint": "coffeelint $(find test src -name '*.coffee')",
        "prepublish": "coffee -o lib -c src",
        "test": "bash scripts/test.sh"
    },
    "version": "0.6.11"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
