# RUTfunctions

[![Build Status](https://travis-ci.org/claudioDcv/RUTfunctions.svg?branch=master)](https://travis-ci.org/claudioDcv/RUTfunctions)

[![codecov](https://codecov.io/gh/claudioDcv/RUTfunctions/branch/master/graph/badge.svg)](https://codecov.io/gh/claudioDcv/RUTfunctions)

Functional helpers for handling RUT Chile written in `ES6` without dependencies

> Helpers funcionales para manipulación de RUT Chileno escritos en `ES6` sin dependencias

--------------------------------------------------------------------------------

## Install NPM

`npm install rutfunctions`

## Install YARN

`yarn add rutfunctions`

## How to Test

Run one, or a combination of the following commands to lint and test your code:

- npm run lint -- lint the source code with ESLint
- npm test -- run unit tests with Mocha
- npm run test:watch -- run unit tests with Mocha, and watch files for changes
- npm run test:cover -- run unit tests with code coverage by Istanbul

## Base in <https://github.com/kriasoft/babel-starter-kit>

## Using:

- RUTclean

```
@param paramrut {string}= 16.761.256-9
@return {string} = 167512569
```

- RUTvalidate

```
@param paramrut {string} = 16.761.256-9
@return {boolean} = true
```

```javascript
// Example
RUTvalidate('167512569')
true
RUTvalidate('167512568')
false
RUTvalidate('16.751.256-8')
false
RUTvalidate('16.751.256-9')
true
```

- RUTformat

```
@param paramrut {number/string} = 167512569
@return {string} = 16.761.256-9
```

- RUTgetDv

```
@param paramrut {number/string} = 16751256 / 16.751.256
@return {string} = 9
```

- RUTnumber

```
@param paramrut {string} = 16.751.256-9 / 16751256-9
@return {string} = 16751256
```

- RUTDv

```
@param paramrut {string} = 16.751.256-9 / 16751256-9
@return {string} = 9
```

- RUTNumAppendDv

```
@param paramrut {string} = 16751256
@return {string} = 167512569
```
