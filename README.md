Forked from https://github.com/danfinlay/eth-ens-namehash, and made the following changes:

1) replaced idna-uts46 with idna-uts46-hx
2) changed one line in eth-ens-namehash to downgrade ES6 stringinterpolation to ES5 string concatenation

Refer to the source for full functional description: 
# Eth ENS Namehash [![CircleCI](https://circleci.com/gh/flyswatter/eth-ens-namehash.svg?style=svg)](https://circleci.com/gh/flyswatter/eth-ens-namehash)

[Available on NPM](https://www.npmjs.com/package/eth-ens-namehash-ms)

## Installation

`npm install eth-ens-namehash-ms -S`

## Usage

```javascript
var namehash = require('eth-ens-namehash-ms')
var hash = namehash.hash('foo.eth')
// '0xde9b09fd7c5f901e23a3f19fecc54828e9c848539801e86591bd9801b019f84f'

// Also supports normalizing strings to ENS compatibility:
var input = getUserInput()
var normalized = namehash.normalize(input)
```

