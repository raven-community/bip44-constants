# BIP44 Constants

This package provides BIP44 coin constants as found here: https://github.com/satoshilabs/slips/blob/master/slip-0044.md

You can read more about [BIP44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki).


## Install
```
npm i --save bip44-constants
```

## Usage
```js
const constants = require('bip44-constants')
console.log(constants)

// iterate through constants
Object.keys(constants).forEach(coinSymbol => {
  const constant = constants[coinSymbol]

  // ...
  console.log(coinSymbol, constant)
})

console.log(constants['LTC'])
// => 2147483650   // equivalent to 0x80000002
```


## Contributors
If you notice that `index.js` is out of date, please run `npm run update` and submit a pull request!
Alternatively,  please submit an issue to notify us that is out of date.


## LICENSE [MIT](LICENSE)
