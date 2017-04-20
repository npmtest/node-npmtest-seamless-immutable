# npmtest-seamless-immutable

#### basic test coverage for  [seamless-immutable (v7.1.2)](https://github.com/rtfeldman/seamless-immutable)  [![npm package](https://img.shields.io/npm/v/npmtest-seamless-immutable.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-seamless-immutable) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-seamless-immutable.svg)](https://travis-ci.org/npmtest/node-npmtest-seamless-immutable)

#### Immutable data structures for JavaScript which are backwards-compatible with normal JS Arrays and Objects.

[![NPM](https://nodei.co/npm/seamless-immutable.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/seamless-immutable)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-seamless-immutable/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-seamless-immutable/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-seamless-immutable/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-seamless-immutable/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-seamless-immutable/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-seamless-immutable/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-seamless-immutable/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-seamless-immutable/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-seamless-immutable/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-seamless-immutable/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-seamless-immutable/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-seamless-immutable/build/test-report.html](https://npmtest.github.io/node-npmtest-seamless-immutable/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-seamless-immutable/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-seamless-immutable/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-seamless-immutable/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-seamless-immutable/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-seamless-immutable/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-seamless-immutable/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-seamless-immutable/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-seamless-immutable/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "seamless-immutable",
    "version": "7.1.2",
    "description": "Immutable data structures for JavaScript which are backwards-compatible with normal JS Arrays and Objects.",
    "main": "src/seamless-immutable.js",
    "browser": "seamless-immutable.development.js",
    "react-native": "src/seamless-immutable.js",
    "devDependencies": {
        "chai": "3.5.0",
        "coveralls": "2.11.8",
        "deep-equal": "1.0.1",
        "envify": "3.4.0",
        "grunt": "0.4.5",
        "grunt-contrib-uglify": "0.11.1",
        "grunt-mocha-test": "0.12.7",
        "istanbul": "0.4.2",
        "jscheck": "0.2.0",
        "lodash": "3.10.1",
        "mocha": "2.4.5",
        "mocha-istanbul": "0.2.0",
        "mocha-lcov-reporter": "1.2.0",
        "react": "^15.0.1",
        "zuul": "3.11.1"
    },
    "scripts": {
        "test": "grunt",
        "test-watch": "mocha --watch test/*.spec.js",
        "jshint": "jshint seamless-immutable.development.js",
        "coverage": "export ISTANBUL_REPORTERS=text-summary,html,lcov && rm -rf tmp/ && rm -rf html-report/ && istanbul instrument test/ -o tmp/ && mocha --reporter mocha-istanbul tmp/*.spec.js && echo Open html-report/index.html to view results as HTML.",
        "zuul": "zuul -- test/*.spec.js",
        "zuul-local": "zuul --local -- test/*.spec.js",
        "travis-test": "npm run jshint && npm test && npm run zuul && npm run coveralls",
        "coveralls": "istanbul cover ./node_modules/mocha/bin/_mocha --report lcovonly -- -R spec && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/rtfeldman/seamless-immutable.git"
    },
    "keywords": [
        "immutable"
    ],
    "author": "Richard Feldman",
    "license": "BSD-3-Clause",
    "bugs": {
        "url": "https://github.com/rtfeldman/seamless-immutable/issues"
    },
    "jshintConfig": {
        "newcap": false,
        "validthis": true,
        "proto": true
    },
    "homepage": "https://github.com/rtfeldman/seamless-immutable"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
