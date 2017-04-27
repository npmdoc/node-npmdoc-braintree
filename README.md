# npmdoc-braintree

#### basic api documentation for  [braintree (v2.0.2)](http://github.com/braintree/braintree_node)  [![npm package](https://img.shields.io/npm/v/npmdoc-braintree.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-braintree) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-braintree.svg)](https://travis-ci.org/npmdoc/node-npmdoc-braintree)

#### A library for integrating with Braintree.

[![NPM](https://nodei.co/npm/braintree.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/braintree)

- [https://npmdoc.github.io/node-npmdoc-braintree/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-braintree/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-braintree/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-braintree/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-braintree/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-braintree/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Braintree",
        "url": "http://www.braintreepayments.com"
    },
    "bugs": {
        "url": "https://github.com/braintree/braintree_node/issues"
    },
    "dependencies": {
        "dateformat": "1.0.1-1.2.3",
        "depd": "~1.1.0",
        "readable-stream": "1.1.10",
        "semver": "5.1.0",
        "source-map-support": "0.2.9",
        "underscore": "1.8.3",
        "xml2js": "0.1.13"
    },
    "description": "A library for integrating with Braintree.",
    "devDependencies": {
        "chai": "1.5.0",
        "coffee-script": "1.6.1",
        "eslint": "^2.7.0",
        "eslint-config-braintree": "^1.0.2",
        "mocha": "3.2.0"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "3c898c40404969f34d31e158fe0b17c09d7955f5",
        "tarball": "https://registry.npmjs.org/braintree/-/braintree-2.0.2.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "d2e1e52d8bb702f1de261d7ecd4b9165ddaf0436",
    "homepage": "http://github.com/braintree/braintree_node",
    "keywords": [
        "braintree",
        "payments"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "braintree"
        }
    ],
    "name": "braintree",
    "optionalDependencies": {
        "source-map-support": "0.2.9"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/braintree/braintree_node.git"
    },
    "scripts": {
        "lint": "eslint lib/",
        "test": "npm run lint && npm run test:unit",
        "test:integration": "mocha --timeout 60000 --slow 2000 spec/integration --recursive --compilers coffee:coffee-script",
        "test:unit": "mocha spec/unit --recursive --compilers coffee:coffee-script"
    },
    "version": "2.0.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
