# bitcoin-fees

  Get bitcoin fee estimates directly from your full node

## Installation

  Copy `fees` to your bin path

  Required dependencies:

    * bitcoin-cli, running bitcoind
    * curl, sort, sed, column, jq

## Usage

  All arguments are optional

```bash
$ fees [blocks] [estimate_mode] [tx_size_bytes] [fiat_price]
```

  * blocks - number of blocks to look at for fee estimate
  * tx_size_bytes - size of the transaction (default 266)
  * estimate_mode - CONSERVATIVE or ECONOMICAL
  * fiat_price - current BTC price in fiat currency
