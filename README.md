case-camel [![Code Climate](https://codeclimate.com/github/ileri/case-camel/badges/gpa.svg)](https://codeclimate.com/github/ileri/case-camel) [![Build Status](https://travis-ci.org/ileri/case-camel.svg?branch=master)](https://travis-ci.org/ileri/case-camel) [![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/feross/standard)
==============
> Parse and stringify CamelCase strings

Install
--------------
```
$ npm install --save case-camel
```

Usage
--------------
```js
var caseCamel = require('case-camel')

// parse
caseCamel.parse('thisIsAnExample') // ['this', 'is', 'an', 'example']
caseCamel.parseSameCase('thisIsAnExample') // ['this', 'Is', 'An', 'Example']

// stringify
caseCamel.stringify(['this', 'is', 'an', 'example']) // 'thisIsAnExample'
caseCamel.stringify(['This', 'iS', 'An', 'eXample']) // 'ThisiSAnEXample'

// check
caseCamel.is('thisIsAnExample') // true
caseCamel.is('this-is-an-example') // false
```
