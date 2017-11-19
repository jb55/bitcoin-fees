# bitcoin-fees

  Get bitcoin fee estimates directly from your full node

## Example

```bash
$ fees 100 e 300
feerate     blocks  hours  fiat
0.00021095  9       1.5    0.513203379
0.00022140  8       1.33   0.5386263479999999
0.00064270  6       1      1.563573414
0.00100261  4       0.66   2.4391696601999993
0.00149164  2       0.33   3.6288916248
```

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

  * `blocks`: number of blocks to look at for fee estimate
  * `tx_size_bytes`: size of the transaction (default `226`)
  * `estimate_mode`: `c` or `e` for conservative or economical
  * `fiat_price`: current BTC price in fiat currency
