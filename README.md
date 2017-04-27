# npmtest-partition-bundle

#### basic test coverage for  [partition-bundle (v2.5.0)](https://github.com/arian/partition-bundle)  [![npm package](https://img.shields.io/npm/v/npmtest-partition-bundle.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-partition-bundle) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-partition-bundle.svg)](https://travis-ci.org/npmtest/node-npmtest-partition-bundle)

#### A Browserify plugin to pack multiple related modules together and load modules on-demand

[![NPM](https://nodei.co/npm/partition-bundle.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/partition-bundle)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-partition-bundle/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-partition-bundle/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-partition-bundle/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-partition-bundle/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-partition-bundle/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-partition-bundle/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-partition-bundle/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-partition-bundle/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-partition-bundle/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-partition-bundle/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-partition-bundle/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-partition-bundle/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-partition-bundle/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-partition-bundle/build/test-report.html](https://npmtest.github.io/node-npmtest-partition-bundle/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-partition-bundle/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-partition-bundle/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-partition-bundle/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-partition-bundle/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-partition-bundle/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-partition-bundle/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-partition-bundle/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-partition-bundle/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Arian Stolwijk"
    },
    "bugs": {
        "url": "https://github.com/arian/partition-bundle/issues"
    },
    "dependencies": {
        "browser-resolve": "^1.9.1",
        "combine-source-map": "^0.7.1",
        "deps-sort": "^1.3.9",
        "mkdirp": "^0.5.1",
        "object-assign": "^3.0.0",
        "through2": "^2.0.0"
    },
    "description": "A Browserify plugin to pack multiple related modules together and load modules on-demand",
    "devDependencies": {
        "browserify": "^10.2.0",
        "expect.js": "^0.3.1",
        "jshint": "^2.7.0",
        "mocha": "^2.2.5"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "2198caf63a4856e1d01177dd7f5714f1e91abd32",
        "tarball": "https://registry.npmjs.org/partition-bundle/-/partition-bundle-2.5.0.tgz"
    },
    "gitHead": "d726c68a1ea76912ac3c01e41a31463c928de556",
    "homepage": "https://github.com/arian/partition-bundle",
    "keywords": [
        "browserify-plugin",
        "JS Loader",
        "browser",
        "factor-bundle",
        "browserify"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "arian"
        }
    ],
    "name": "partition-bundle",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/arian/partition-bundle.git"
    },
    "scripts": {
        "build-prelude": "browserify preludes/_prelude.js -o preludes/prelude.js",
        "build-test-fixtures": "browserify -d -p [ ./index --map test/fixtures/map.json -o dist --url ../dist ]",
        "build-tests": "browserify test/browser.js -o dist/tests.js",
        "pretest": "rm -rf dist/**/*.js && npm run build-prelude && npm run build-tests && npm run build-test-fixtures",
        "test": "jshint . && mocha test/node"
    },
    "version": "2.5.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
