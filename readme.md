# Crypto Search


## Usage
	
   Include the crypto-search folder in to your project. 
   
Go to your project directory and run following command in command line.   
``` shell
	$ npm install trie-search --save
```

Require the object in your code
``` js
	const cryptoSearch = require('<the folder path>/crypto-search/search')
    
``` 
## Functions and examples:

	
* searchNames(string)
```js
	const cryptoSearch = require('./crypto-search/search')
    
    //searchNames(prefix): Return all the cryptocurrencies' name whose name starts with the given prefix
    
    let names = cryptoSearch.searchNames('BtC');
    console.log(names) // [ 'BTC Lite', 'BTCMoon' ]
```

* searchSymbols(string)
```js

	const cryptoSearch = require('./crypto-search/search')

    //searchSymbols(prefix): Return all the cryptocurrencies' symbol whose symbol starts with the given prefix
    
    let symbols = cryptoSearch.searchSymbols('BtC');
    console.log(symbols) /* [ 'BTC',
                            'BTCL',
                            'BTCL*',
                            'BTCM',
                            'BTCR',
                            'BTCRY',
                            'BTCRED',
                            'BTCA',
                            'BTCN',
                            'BTCC',
                            'BTCH',
                            'BTCP',
                            'BTCS',
                            'BTCS*',
                            'BTCD',
                            'BTCE',
                            'BTCE*',
                            'BTCGO',
                            'BTCZ' ] */
```

* namesToSymbols(string)

```js

	const cryptoSearch = require('./crypto-search/search')
    
    //namesToSymbols(prefix) return all the cryptocurrencies' symbol whose name starts with the given prefix
    
    let symbols = cryptoSearch.namesToSymbols('BtC');
    console.log(symbols) /* [ 'BTCL', 'BTCM' ] */
```

* symbolsToNames(string)

```js

	const cryptoSearch = require('./crypto-search/search')
    
    //symbolsToNames(prefix) return all the cryptocurrencies' name whose symbol starts with the given prefix
    
    let names = cryptoSearch.symbolsToNames('BtC');
    console.log(names) /* [ 'Bitcoin',
                              'BTC Lite',
                              'BitluckCoin',
                              'BTCMoon',
                              'BitCurrency',
                              'BitCrystal',
                              'Bitcoin Red',
                              'Bitair',
                              'BitcoiNote',
                              'Bitcoin Core',
                              'Bitcoin Hush',
                              'Bitcoin Private',
                              'Bitcoin Scrypt',
                              'Bitcoin Supreme',
                              'BitcoinDark',
                              'EthereumBitcoin',
                              'BitcoinEX',
                              'BitcoinGo',
                              'BitcoinZ' ] */
```