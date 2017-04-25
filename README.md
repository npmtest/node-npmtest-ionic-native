# npmtest-ionic-native

#### basic test coverage for  ionic-native (v3.5.0)  [![npm package](https://img.shields.io/npm/v/npmtest-ionic-native.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-ionic-native) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-ionic-native.svg)](https://travis-ci.org/npmtest/node-npmtest-ionic-native)

#### Native plugin wrappers for Cordova and Ionic with TypeScript, ES6+, Promise and Observable support

[![NPM](https://nodei.co/npm/ionic-native.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ionic-native)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-ionic-native/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-ionic-native/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-ionic-native/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-ionic-native/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-ionic-native/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-ionic-native/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-ionic-native/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-ionic-native/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-ionic-native/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-ionic-native/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-ionic-native/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-ionic-native/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-ionic-native/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-ionic-native/build/test-report.html](https://npmtest.github.io/node-npmtest-ionic-native/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-ionic-native/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-ionic-native/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-ionic-native/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ionic-native/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ionic-native/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ionic-native/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-ionic-native/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-ionic-native/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "ionic-native",
    "version": "3.5.0",
    "description": "Native plugin wrappers for Cordova and Ionic with TypeScript, ES6+, Promise and Observable support",
    "license": "MIT",
    "devDependencies": {
        "@angular/compiler": "2.4.8",
        "@angular/compiler-cli": "2.4.8",
        "@angular/core": "2.4.8",
        "canonical-path": "0.0.2",
        "child-process-promise": "2.2.0",
        "conventional-changelog-cli": "1.2.0",
        "cpr": "2.0.2",
        "cz-conventional-changelog": "1.2.0",
        "decamelize": "1.2.0",
        "dgeni": "0.4.7",
        "dgeni-packages": "0.16.10",
        "fs-extra": "2.0.0",
        "fs-extra-promise": "0.4.1",
        "gulp": "3.9.1",
        "gulp-rename": "1.2.2",
        "gulp-replace": "0.5.4",
        "gulp-tslint": "6.1.2",
        "lodash": "4.17.4",
        "minimist": "1.1.3",
        "node-html-encoder": "0.0.2",
        "q": "1.4.1",
        "queue": "4.2.1",
        "rimraf": "2.5.4",
        "rxjs": "5.0.1",
        "semver": "5.3.0",
        "tslint": "3.15.1",
        "tslint-ionic-rules": "0.0.7",
        "typescript": "2.0.09",
        "zone.js": "0.7.2"
    },
    "scripts": {
        "start": "npm run test:watch",
        "lint": "gulp lint",
        "build": "npm run clean && npm run lint && npm run build:core && npm run build:modules",
        "build:core": "ngc -p scripts/build/tsconfig-core.json",
        "build:modules": "node scripts/build/build.js",
        "clean": "rimraf dist .tmp",
        "shipit": "npm run build && gulp readmes && npm run npmpub",
        "npmpub": "node scripts/build/publish.js",
        "changelog": "conventional-changelog -p angular -i CHANGELOG.md -s -r 0",
        "postchangelog": "git commit -am \"chore(): update changelog\""
    },
    "config": {
        "commitizen": {
            "path": "./node_modules/cz-conventional-changelog"
        }
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
