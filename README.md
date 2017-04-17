# test coverage for  [d3-scale (v1.0.5)](https://d3js.org/d3-scale/)  [![npm package](https://img.shields.io/npm/v/npmtest-d3-scale.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-d3-scale) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-d3-scale.svg)](https://travis-ci.org/npmtest/node-npmtest-d3-scale)
#### Encodings that map abstract data to visual representation.

[![NPM](https://nodei.co/npm/d3-scale.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/d3-scale)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-d3-scale/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-d3-scale/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-d3-scale/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-d3-scale/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-d3-scale/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-d3-scale/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-d3-scale/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-d3-scale/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-d3-scale/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-d3-scale/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-d3-scale/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-d3-scale/build/test-report.html](https://npmtest.github.io/node-npmtest-d3-scale/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-d3-scale/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-d3-scale/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-d3-scale/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-d3-scale/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-d3-scale/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-d3-scale/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-d3-scale/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-d3-scale/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mike Bostock",
        "url": "http://bost.ocks.org/mike"
    },
    "bugs": {
        "url": "https://github.com/d3/d3-scale/issues"
    },
    "dependencies": {
        "d3-array": "1",
        "d3-collection": "1",
        "d3-color": "1",
        "d3-format": "1",
        "d3-interpolate": "1",
        "d3-time": "1",
        "d3-time-format": "2"
    },
    "description": "Encodings that map abstract data to visual representation.",
    "devDependencies": {
        "eslint": "3",
        "package-preamble": "0.0",
        "rollup": "0.41",
        "tape": "4",
        "uglify-js": "^2.8.11"
    },
    "directories": {},
    "dist": {
        "shasum": "418506f0fb18eb052b385e196398acc2a4134858",
        "tarball": "https://registry.npmjs.org/d3-scale/-/d3-scale-1.0.5.tgz"
    },
    "gitHead": "4a35a24fb10ac8e45529dc184d0c94437decd1cf",
    "homepage": "https://d3js.org/d3-scale/",
    "jsnext:main": "index",
    "keywords": [
        "d3",
        "d3-module",
        "scale",
        "visualization"
    ],
    "license": "BSD-3-Clause",
    "main": "build/d3-scale.js",
    "maintainers": [
        {
            "name": "mbostock"
        }
    ],
    "module": "index",
    "name": "d3-scale",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/d3/d3-scale.git"
    },
    "scripts": {
        "postpublish": "git push && git push --tags && cd ../d3.github.com && git pull && cp ../d3-scale/build/d3-scale.js d3-scale.v1.js && cp ../d3-scale/build/d3-scale.min.js d3-scale.v1.min.js && git add d3-scale.v1.js d3-scale.v1.min.js && git commit -m \"d3-scale ${npm_package_version}\" && git push && cd - && zip -j build/d3-scale.zip -- LICENSE README.md build/d3-scale.js build/d3-scale.min.js",
        "prepublish": "npm run test && uglifyjs --preamble \"$(preamble)\" build/d3-scale.js -c -m -o build/d3-scale.min.js",
        "pretest": "rm -rf build && mkdir build && rollup --banner \"$(preamble)\" -f umd -g d3-array:d3,d3-collection:d3,d3-color:d3,d3-format:d3,d3-interpolate:d3,d3-time:d3,d3-time-format:d3 -n d3 -o build/d3-scale.js -- index.js",
        "test": "TZ=America/Los_Angeles tape 'test/**/*-test.js' && eslint index.js src test"
    },
    "version": "1.0.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
