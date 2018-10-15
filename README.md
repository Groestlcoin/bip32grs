# bip32
[![Build Status](https://travis-ci.org/bitcoinjs/bip32.png?branch=master)](https://travis-ci.org/bitcoinjs/bip32)

[![NPM](https://img.shields.io/npm/v/bip32.svg)](https://www.npmjs.org/package/bip32)

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

A [BIP32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki) compatible library.


## Example
``` javascript
let bip32grs = require('bip32grs')
let node = bip32grs.fromBase58('xprv9s21ZrQH143K3XpLJrX92hM28H2o1CgVi6HXCWGBXtMkHxSkpxiFcnmzjy5qNyi3QUfSVXXapRT8St3wyLbWux9JysZZgvmvQZ75FUqrakP')

let child = node.derivePath('m/0/0')
// ...
```

## LICENSE [MIT](LICENSE)
A derivation (and extraction for modularity) of the `HDWallet`/`HDNode` written and tested by [bitcoinjs-lib](https://github.com/bitcoinjs/bitcoinjs-lib) contributors since 2014.
