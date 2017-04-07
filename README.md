# api documentation for  [jscpd (v0.6.10)](https://github.com/kucherenko/jscpd#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-jscpd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jscpd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jscpd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jscpd)
#### Copy/paste detector for programming code, support JavaScript, CoffeeScript, PHP, Ruby, Python, Less, Go, Java, Yaml, C#, C++, C, Puppet, Twig languages

[![NPM](https://nodei.co/npm/jscpd.png?downloads=true)](https://www.npmjs.com/package/jscpd)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jscpd/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-jscpd_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jscpd/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jscpd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jscpd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrey Kucherenko",
        "email": "kucherenko.andrey@gmail.com",
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
        "crypto": ">=0.0.x",
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
        "coveralls": "2.11.x",
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
        "shasum": "bb76eb4fe70458481a28189870065164105d931a",
        "tarball": "https://registry.npmjs.org/jscpd/-/jscpd-0.6.10.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "d0cd0d298f696d8d2e78cb405b58b20e4580eb75",
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
            "name": "apk",
            "email": "kucherenko.andrey@gmail.com"
        }
    ],
    "name": "jscpd",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
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
    "version": "0.6.10"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jscpd](#apidoc.module.jscpd)
1.  object <span class="apidocSignatureSpan">jscpd.</span>clone
1.  object <span class="apidocSignatureSpan">jscpd.</span>detector
1.  object <span class="apidocSignatureSpan">jscpd.</span>map
1.  object <span class="apidocSignatureSpan">jscpd.</span>report
1.  object <span class="apidocSignatureSpan">jscpd.</span>strategy

#### [module jscpd.clone](#apidoc.module.jscpd.clone)
1.  [function <span class="apidocSignatureSpan">jscpd.clone.</span>Clone (firstFile, secondFile, firstFileStart, secondFileStart, linesCount, tokensCount)](#apidoc.element.jscpd.clone.Clone)

#### [module jscpd.detector](#apidoc.module.jscpd.detector)
1.  [function <span class="apidocSignatureSpan">jscpd.detector.</span>Detector (strategy)](#apidoc.element.jscpd.detector.Detector)

#### [module jscpd.map](#apidoc.module.jscpd.map)
1.  [function <span class="apidocSignatureSpan">jscpd.map.</span>Map ()](#apidoc.element.jscpd.map.Map)

#### [module jscpd.report](#apidoc.module.jscpd.report)
1.  [function <span class="apidocSignatureSpan">jscpd.report.</span>Report (options)](#apidoc.element.jscpd.report.Report)

#### [module jscpd.strategy](#apidoc.module.jscpd.strategy)
1.  [function <span class="apidocSignatureSpan">jscpd.strategy.</span>Strategy (options)](#apidoc.element.jscpd.strategy.Strategy)



# <a name="apidoc.module.jscpd"></a>[module jscpd](#apidoc.module.jscpd)



# <a name="apidoc.module.jscpd.clone"></a>[module jscpd.clone](#apidoc.module.jscpd.clone)

#### <a name="apidoc.element.jscpd.clone.Clone"></a>[function <span class="apidocSignatureSpan">jscpd.clone.</span>Clone (firstFile, secondFile, firstFileStart, secondFileStart, linesCount, tokensCount)](#apidoc.element.jscpd.clone.Clone)
- description and source-code
```javascript
function Clone(firstFile, secondFile, firstFileStart, secondFileStart, linesCount, tokensCount) {
  this.firstFile = firstFile;
  this.secondFile = secondFile;
  this.firstFileStart = firstFileStart;
  this.secondFileStart = secondFileStart;
  this.linesCount = linesCount;
  this.tokensCount = tokensCount;
  this.firstFileAnnotatedCode = {};
  this.secondFileAnnotatedCode = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jscpd.detector"></a>[module jscpd.detector](#apidoc.module.jscpd.detector)

#### <a name="apidoc.element.jscpd.detector.Detector"></a>[function <span class="apidocSignatureSpan">jscpd.detector.</span>Detector (strategy)](#apidoc.element.jscpd.detector.Detector)
- description and source-code
```javascript
function Detector(strategy) {
  this.strategy = strategy;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jscpd.map"></a>[module jscpd.map](#apidoc.module.jscpd.map)

#### <a name="apidoc.element.jscpd.map.Map"></a>[function <span class="apidocSignatureSpan">jscpd.map.</span>Map ()](#apidoc.element.jscpd.map.Map)
- description and source-code
```javascript
function Map() {
  this.clones = [];
  this.clonesByFile = {};
  this.numberOfDuplication = 0;
  this.numberOfLines = 0;
  this.numberOfFiles = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jscpd.report"></a>[module jscpd.report](#apidoc.module.jscpd.report)

#### <a name="apidoc.element.jscpd.report.Report"></a>[function <span class="apidocSignatureSpan">jscpd.report.</span>Report (options)](#apidoc.element.jscpd.report.Report)
- description and source-code
```javascript
function Report(options) {
  var cwd, ext, isAbsolute, reporter;
  this.options = options;
  reporter = this.options.reporter;
  if (this.options.output) {
    ext = this.options.output.split('.').pop();
  }
  if (ext === 'xml' && reporter === 'json' || ext === 'json' && reporter === 'xml') {
    logger.warn("output file extention '" + this.options.output + "' does not match reporter '" + reporter + "'");
  }
  switch (reporter) {
    case 'xml':
      reporter = './reporters/xml-pmd';
      break;
    case 'json':
      reporter = './reporters/json';
      break;
    default:
      cwd = process.cwd();
      reporter = path.normalize(reporter);
      isAbsolute = reporter.indexOf(cwd) === 0;
      if (!isAbsolute) {
        reporter = path.join(cwd, reporter);
      }
  }
  this.reporter = require(reporter);
  this.stdReporter = require('./reporters/_std-log');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jscpd.strategy"></a>[module jscpd.strategy](#apidoc.module.jscpd.strategy)

#### <a name="apidoc.element.jscpd.strategy.Strategy"></a>[function <span class="apidocSignatureSpan">jscpd.strategy.</span>Strategy (options)](#apidoc.element.jscpd.strategy.Strategy)
- description and source-code
```javascript
function Strategy(options) {
  this.options = options;
  this.languages = options.languages;
  this.storage = new Storage();
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
